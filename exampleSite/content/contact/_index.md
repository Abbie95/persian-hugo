---
title: Contact
description: contact me form
data_2: Name
data_4: Email
data_5: Phone Number
data_12: How do you prefer to be contacted?
data_13: 'Type of shoot interested in:'
data_14: Desired Date
data_15: Desired Location
data_11: Comments and Questions
menu:
  main:
    weight: 4

---
<form method="post" name="contact form" action="/thank-you"  onSubmit="return validateForm();" data-netlify="true">

<input type="hidden" name="form-name" value="contact form" />  
<div style="max-width: 400px;">  
</div>  
<div style="padding-bottom: 18px;font-size : 36px;">Contact Me</div>  
<p style="max-width : 600px;font-size : 12px;">Hello friend! Before I book a shoot, I like to make sure I have gotten to know you a little and know your goals for your shoot! I want to make each shoot as personalized to you and your style as possible. Start here, and I will send you a message soon! I look foward to talking to you!</p>  
<div style="display: flex; padding-bottom: 18px;max-width : 550px;">  
<div style=" margin-left: 0; margin-right: 1%; width: 49%;">Name<span style="color: red;"> *</span><br/>  
<input type="text" id="data_2" name="data_2" style="max-width: 100%;" class="form-control"/>  
</div>  
<div style=" margin-left: 1%; margin-right: 0; width: 49%;">Last name<span style="color: red;"> *</span><br/>  
<input type="text" id="data_3" name="data_3" style="max-width: 100%;" class="form-control"/>  
</div>  
</div><div style="padding-bottom: 18px;">Email<span style="color: red;"> *</span><br/>  
<input type="text" id="data_4" name="data_4" style="max-width : 550px;" class="form-control"/>  
</div>  
<div style="padding-bottom: 18px;">Phone number<br/>  
<input type="text" id="data_5" name="data_5" style="max-width : 550px;" class="form-control"/>  
</div>  
<div style="padding-bottom: 18px;">How do you prefer to be contacted?<span style="color: red;"> *</span><br/>  
<span><input type="checkbox" id="data_12_0" name="data_12" value="Text"/> Text</span><br/>  
<span><input type="checkbox" id="data_12_1" name="data_12" value="Email"/> Email</span><br/>  
</div>  
<div style="padding-bottom: 18px;">Type of shoot interested in:<span style="color: red;"> *</span><br/>  
<textarea id="data_13" false name="data_13" style="max-width : 450px;" rows="2" class="form-control"></textarea>  
</div>  
<div style="padding-bottom: 18px;">Desired Date<br/>  
<input type="text" id="data_14" name="data_14" style="max-width : 450px;" class="form-control"/>  
</div>  
<div style="padding-bottom: 18px;">Desired Location<br/>  
<input type="text" id="data_15" name="data_15" style="max-width : 450px;" class="form-control"/>  
</div>  
<div style="padding-bottom: 18px;">Comments and Questions<br/>  
<textarea id="data_11" false name="data_11" style="max-width : 550px;" rows="6" class="form-control"></textarea>  
</div>  
<div style="padding-bottom: 18px;"><input name="skip_Submit" value="Submit" type="submit"/></div>  
<div>  
<div style="float:right"><a href="[https://www.100forms.com](https://www.100forms.com "https://www.100forms.com")" id="lnk100" title="form to email">form to email</a></div>  
<script src="[https://www.100forms.com/js/FORMKEY:72UM3XRW3J6L](https://www.100forms.com "https://www.100forms.com")" type="text/javascript"></script>  
</div>  
</form>

<script type="text/javascript">  
function validateForm() {  
if (isEmpty(document.getElementById('data_2').value.trim())) {  
alert('First name is required!');  
return false;  
}  
if (isEmpty(document.getElementById('data_3').value.trim())) {  
alert('Last name is required!');  
return false;  
}  
if (isEmpty(document.getElementById('data_4').value.trim())) {  
alert('Email is required!');  
return false;  
}  
if (!validateEmail(document.getElementById('data_4').value.trim())) {  
alert('Email must be a valid email address!');  
return false;  
}  
if (!document.getElementById('data_12_0').checked && !document.getElementById('data_12_1').checked ) {  
alert('How do you prefer to be contacted? is required!');  
return false;}  
if (isEmpty(document.getElementById('data_13').value.trim())) {  
alert('Type of shoot interested in: is required!');  
return false;  
}  
return true;  
}  
function isEmpty(str) { return (str.length === 0 || !str.trim()); }  
function validateEmail(email) {  
var re = /^(\[\\w-\]+(?:\\.\[\\w-\]+)_)@((?:\[\\w-\]+\\.)_\\w\[\\w-\]{0,66})\\.(\[a-z\]{2,15}(?:\\.\[a-z\]{2})?)$/i;  
return isEmpty(email) || re.test(email);  
}  
</script>