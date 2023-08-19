<template>
   <div class="login">
    <div class="main">
      <h1>Reset Password</h1>
      <form class="form-horizontal">
        <div class="form-group">
          <label class="content control-label">Email</label>
          <div class="form-input">
            <input
              type="text"
              placeholder="Email"
              class="form-control"
            />
            <span></span>
          </div>
        </div>

        <div
          id="rc-anchor-container"
          class="rc-anchor rc-anchor-normal rc-anchor-light"
        >
          <input
            type="checkbox"
            class="recaptcha-checkbox goog-inline-block recaptcha-checkbox-unchecked rc-anchor-checkbox"
            role="checkbox"
            aria-checked="false"
            id="recaptcha-anchor" tabindex="0" dir="ltr" aria-labelledby="recaptcha-anchor-label"/>
           <div class="recaptcha-checkbox-border" role="presentation"></div>
          <div class="recaptcha-checkbox-spinner" role="presentation">
            <div class="recaptcha-checkbox-spinner-overlay"></div>
          </div>
          <div class="recaptcha-checkbox-checkmark" role="presentation"></div>

          <label class="rc-anchor-center-item rc-anchor-checkbox-label" aria-hidden="true" role="presentation" id="recaptcha-anchor-label">
            <span></span>Tôi không phải là người máy
          </label>
          <div class="rc-anchor-normal-footer">
            <div class="rc-anchor-logo-portrait" aria-hidden="true" role="presentation">
              <div class="rc-anchor-logo-img rc-anchor-logo-img-portrait"></div>
              <div class="rc-anchor-logo-text">reCAPTCHA</div>
            </div>
            <div class="rc-anchor-pt">
              <a href="https://www.google.com/intl/vi/policies/privacy/" target="_blank">Bảo mật</a>
              <span aria-hidden="true" role="presentation"> - </span>
              <a href="https://www.google.com/intl/vi/policies/terms/" target="_blank">Điều khoản</a
              >
            </div>
          </div>
        </div>

        <div class="button-from">
          <button type="submit" class="create-button b2">Reset Password</button>
          <a href="" class="forgot">  Back to login</a>
        </div>
      </form>
    </div>
</div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style scoped>
.login{
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 14px;
  color: #333;
  margin-top: 50px;
  margin-left: 200px;
}

h1 {
  margin-top: 20px;
  font-size: 30px;
  margin-bottom: 0.8em;
}

.form-horizontal .control-label {
  padding-top: 7px;
  margin-bottom: 0;
  float: left;
  text-align: left;
}

.form-group {
  display: table;
  margin-left: 100px;
  margin-bottom: 30px;
}

.content  {
  position: relative;
  min-height: 1px;
  padding-right: 15px;
  padding-left: 15px;
  font-weight: bold;
}

.form-input {
  width: max-content;
  float: right;
  position: relative;
  min-height: 1px;
  padding-right: 15px;
  padding-left: 15px;
}

.form-control {
  display: block;
  width: 500px;
  height: 20px;
  padding: 6px 12px;
  font-size: 16px;
  color: #555;
  background-color: #fff;
  border: 1px solid #ccc;
  border-radius: 4px;
  
}

/* reCAPTCHA */

#rc-anchor-container {
  background: #f9f9f9;
  border: 1px solid #d3d3d3;
  padding: 10px;
  height: 56px;
  width: 280px;
  font-family: Arial, sans-serif;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  margin-left: 205px;
  border-radius: 5px;
}

/* Styles for the checkbox holder */
.rc-anchor-checkbox-holder {
  display: flex;
  align-items: center;
  margin-right: 10px;
}

/* Styles for the checkbox */
.recaptcha-checkbox {
  display: inline-block;
  width: 20px;
  height: 20px;
  border: 1px solid #999;
  background-color: #fff;
  position: relative;
  cursor: pointer;
}

.recaptcha-checkbox:hover {
  border-color: #555;
}

/* Styles for the checkmark icon */
.recaptcha-checkbox-checkmark {
  width: 9px;
  height: 15px;
  border: solid #0f9d58;
  border-width: 0 2px 2px 0;
  transform: rotate(45deg);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: none;
}

.rc-anchor-checkbox-label {
  width: 152px;
  display: inline-block;
  vertical-align: middle;
  font-size: 14px;
  color: #333;
  font-weight: 400;
  line-height: 17px;
}

.rc-anchor-normal-footer {
  font-size: 12px;
  color: #777;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 10px;
}

.rc-anchor-pt a {
  text-decoration: none;
  color: #777;
  font-size: 7px;
  display: inline;
  padding-left: 1px;
  padding-right: 1px;
  padding-top: 2px;
  padding-bottom: 2px;
  
}

.rc-anchor-pt a:hover {
  color: #0f9d58;
}
.rc-anchor-logo-img {
  background-image: url("https://www.gstatic.com/recaptcha/api2/logo_48.png");
  width: 32px;
  height: 32px;
  background-size: 32px;
  margin: 0 13px 0 13px;
  display: inline-block;
  vertical-align: middle;
}

.rc-anchor-checkbox-holder {
  display: flex;
  align-items: center;
}

.rc-anchor-checkbox-label {
  margin-left: 10px;
}

/* */
.button-from {
  padding-top: 15px;
  margin-left: 115px;
}
.create-button {
  background: #337ab7;
  color: #fff;
  border: none;
  border-radius: 4px;
  width: 150px;
  height: 32px;
  font-size: 14px;
  padding: 6px 12px;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.3);
  text-align: center;
  position: relative;
  left: 90px;
}

.create-button:hover {
  background-color: #3275fc;
}
.forgot {
  margin-left: 100px;
  text-decoration: none;
  color: #10589b;
}
.forgot:hover{
  color: #3275fc;
}
label {
  text-align: left;
}


</style>