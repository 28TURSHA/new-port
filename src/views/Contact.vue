<template>
  <body>
    <div class="container">
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 text-center">
          <h2 class="form-title">Get in touch</h2>
          <br /><br />
        </div>
      </div>
      <div class="row">
        <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12">
          <form
            @submit.prevent="handleSubmit"
            id="contact-form"
            name="myForm"
            class="form"
            action="#"
            onsubmit="return validateForm()"
            method="POST"
            role="form"
          >
            <div class="form-group">
              <label class="form-label" id="nameLabel" for="name"></label>
              <input
                type="text"
                class="form-control"
                id="name"
                name="name"
                placeholder="Your name"
                tabindex="1"
                v-model="name"
                required
              />
            </div>

            <div class="form-group">
              <label class="form-label" id="emailLabel" for="email"></label>
              <input
                type="email"
                class="form-control"
                id="email"
                name="email"
                placeholder="Your Email"
                tabindex="2"
                v-model="email"
                required
              />
            </div>

            <div class="form-group">
              <label class="form-label" id="subjectLabel" for="sublect"></label>
              <input
                type="text"
                class="form-control"
                id="subject"
                name="subject"
                placeholder="Subject"
                tabindex="3"
                v-model="subject"
                required
              />
            </div>

            <div class="form-group">
              <label class="form-label" id="messageLabel" for="message"></label>
              <textarea
                rows="6"
                cols="60"
                name="message"
                class="form-control"
                id="message"
                placeholder="Your message"
                tabindex="4"
                v-model="message"
                required
              ></textarea>
            </div>
            <br />

            <div class="text-center margin-top-25">
              <button type="submit" class="btn btn-mod btn-border btn-large">
                Send Message</button
              ><br /><br />
            </div>
          </form>
          <!-- End form -->
        </div>
        <!-- End col -->
      </div>
      <!-- End row --><br /><br />

      <div class="contact row">
        <div class="icon col-md-4 col-lg-4" style="color: #000">
          <i class="fas fa-phone-alt"></i>
          <br />
          <div class="call-me fw-bold">Contact Number:</div>
          <div class="call-me-1 text-muted">+(27) 67 668 5517</div>
        </div>

        <div class="icon col-md-4 col-lg-4" style="color: #000">
          <i class="fas fa-map-marker-alt"></i>
          <br />
          <div class="call-me fw-bold">Location:</div>
          <div class="call-me-1 text-muted">Cape Town, South Africa</div>
        </div>

        <div class="icon col-md-4 col-lg-4" style="color: #000">
          <i class="fas fa-envelope"></i>
          <br />
          <div class="call-me fw-bold">Email Address:</div>
          <div class="call-me-1 text-muted">turshaarendse@gmail.com</div>
        </div>
      </div>
    </div>
    <!-- End container -->
  </body>
  <!-- End body -->
</template>

<script>
export default {
  data() {
    return {
      name: "",
      email: "",
      subject: "",
      message: "",
    };
  },
  methods: {
    handleSubmit() {
      console.log(this.name, this.email, this.subject, this.message);
      fetch("https://backend-tursha.herokuapp.com/contact", {
        method: "POST",
        body: JSON.stringify({
          name: this.name,
          email: this.email,
          subject: this.subject,
          message: this.message,
        }),
        headers: {
          "Content-type": "application/json; charset=UTF-8",
        },
      })
        .then((response) => response.json())
        .then((json) => alert(json.msg))
        .catch((e) => alert(e.msg));
    },
  },
};
</script>
<style scoped>
#success-message {
  opacity: 0;
}

.col-xs-12.col-sm-12.col-md-12.col-lg-12 {
  padding: 0 20% 0 20%;
}

.margin-top-25 {
  margin-top: 25px;
}

.form-title {
  color: black;
  padding-top: 140px;
  font-size: 45px;
  font-weight: 300;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}

.form-group .form-control {
  border-bottom: 1px;
  border-style: none none solid none;
  border-radius: 0;
  border-color: #000;
}

.form-group .form-control:focus {
  box-shadow: none;
  border-width: 0 0 2px 0;
  border-color: #000;
}

textarea {
  resize: none;
}

.btn-mod.btn-large {
  height: auto;
  padding: 13px 52px;
  font-size: 15px;
}

.btn-mod.btn-border {
  color: #000000;
  border: 1px solid #000000;
  background: transparent;
}

.btn-mod,
a.btn-mod {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  padding: 4px 13px;
  color: #fff;
  background: rgba(34, 34, 34, 0.9);
  border: 1px solid transparent;
  font-size: 11px;
  font-weight: 400;
  text-transform: uppercase;
  text-decoration: none;
  letter-spacing: 2px;
  -webkit-border-radius: 0;
  -moz-border-radius: 0;
  border-radius: 0;
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  box-shadow: none;
  -webkit-transition: all 0.2s cubic-bezier(0, 0, 0.58, 1);
  -moz-transition: all 0.2s cubic-bezier(0, 0, 0.58, 1);
  -o-transition: all 0.2s cubic-bezier(0, 0, 0.58, 1);
  -ms-transition: all 0.2s cubic-bezier(0, 0, 0.58, 1);
  transition: all 0.2s cubic-bezier(0, 0, 0.58, 1);
}

.btn-mod.btn-border:hover,
.btn-mod.btn-border:active,
.btn-mod.btn-border:focus,
.btn-mod.btn-border:active:focus {
  color: #fff;
  border-color: #000;
  background: #000;
  outline: none;
}

@media only screen and (max-width: 500px) {
  .btn-mod.btn-large {
    padding: 6px 16px;
    font-size: 11px;
  }

  .form-title {
    font-size: 20px;
  }
}
.fas {
  font-size: 30px;
}
</style>
