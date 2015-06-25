# jQuery jFormFill
Fill a form from json or copy from another form
##Usage
include jquery and jquery.JformFill.js
###Fill from another form
Inside each form element put attribute <code>data-fill="name"</code>
"name" is name of any element you want to copy from

<pre><code>
$(form).jFormFill()
</code></pre>
####Live Fill
if you want to fill a form whenever other element changes
put attribute<code> data-live-fill="true"</code> in < form >tag
<pre><code>
$(form).jFormFill()
</code></pre>

###Fill from json
To Fill a form from json 
<pre><code>
var json={name:value,name2:value2}
$(form).jFormFill(json)
</code></pre>
name is name of form element
####Ajax
<pre><code>$(form).jFormFill("http://example.com/data.json")
here this url should output name value pair</code></pre>
####Events
Event when finished filling
<code>jform.fill</code>
<pre><code>
$(form).on('jform.fill',function(){
             
})
</code></pre>