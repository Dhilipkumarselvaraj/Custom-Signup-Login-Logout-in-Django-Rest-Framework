<h1 class="code-line" data-line-start=1 data-line-end=2 ><a id="Custom_Signup_Login_Logout_with_Django_Rest_Framework_1"></a>Custom Signup, Login, Logout with Django Rest Framework:</h1>
<p class="has-line-data" data-line-start="3" data-line-end="4">NOTE:</p>
<ul>
<li class="has-line-data" data-line-start="4" data-line-end="6">signup, login, logout works based on email and password.</li>
</ul>
<h1 class="code-line" data-line-start=6 data-line-end=7 ><a id="Signup_6"></a>Signup:</h1>
<p class="has-line-data" data-line-start="7" data-line-end="10"><strong>URL:</strong> <a href="http://localhost:8000/account/signup/">http://localhost:8000/account/signup/</a><br>
<strong>Method:</strong>    POST<br>
<strong>Header:</strong></p>
<ul>
<li class="has-line-data" data-line-start="10" data-line-end="12">Content-Type - application/json</li>
</ul>
<p class="has-line-data" data-line-start="12" data-line-end="13"><strong>Payload:</strong></p>
<pre><code class="has-line-data" data-line-start="14" data-line-end="22">    {
        &quot;email&quot;:&quot;user1@user1.com&quot;,
        &quot;username&quot;:&quot;user1&quot;,
        &quot;password&quot;:&quot;admin&quot;,
        &quot;password2&quot;:&quot;admin&quot;
    }

</code></pre>
<p class="has-line-data" data-line-start="22" data-line-end="23"><strong>Response:</strong></p>
<pre><code class="has-line-data" data-line-start="24" data-line-end="31">    {
        &quot;response&quot;: &quot;successfully created&quot;,
        &quot;email&quot;: &quot;user1@user1.com&quot;,
        &quot;username&quot;: &quot;user1&quot;
    }

</code></pre>
<hr>
<h1 class="code-line" data-line-start=33 data-line-end=34 ><a id="Login_33"></a>Login:</h1>
<p class="has-line-data" data-line-start="34" data-line-end="37"><strong>URL:</strong> <a href="http://localhost:8000/account/login/">http://localhost:8000/account/login/</a><br>
<strong>Method:</strong> POST<br>
<strong>Header:</strong></p>
<ul>
<li class="has-line-data" data-line-start="37" data-line-end="39">Content-Type - application/json</li>
</ul>
<p class="has-line-data" data-line-start="39" data-line-end="40"><strong>Payload:</strong></p>
<pre><code class="has-line-data" data-line-start="41" data-line-end="47">    {
        &quot;email&quot;:&quot;user1@user1.com&quot;,
        &quot;password&quot;:&quot;admin&quot;
    }

</code></pre>
<p class="has-line-data" data-line-start="47" data-line-end="48"><strong>Response:</strong></p>
<pre><code class="has-line-data" data-line-start="49" data-line-end="56">    {
    &quot;reponse&quot;: &quot;success&quot;,
    &quot;response_message&quot;: &quot;successfully logged in.&quot;,
    &quot;error_message&quot;: &quot;no error.&quot;
    }

</code></pre>
<hr>
<h1 class="code-line" data-line-start=58 data-line-end=59 ><a id="Logout_58"></a>Logout:</h1>
<p class="has-line-data" data-line-start="59" data-line-end="62"><strong>URL:</strong> <a href="http://localhost:8000/account/logout/">http://localhost:8000/account/logout/</a><br>
<strong>Method:</strong> POST<br>
<strong>Header:</strong></p>
<ul>
<li class="has-line-data" data-line-start="62" data-line-end="64">Content-Type - application/json</li>
</ul>
<p class="has-line-data" data-line-start="64" data-line-end="65"><strong>Payload:</strong></p>
<pre><code class="has-line-data" data-line-start="66" data-line-end="72">    {
        &quot;email&quot;:&quot;user1@user1.com&quot;,
        &quot;password&quot;:&quot;admin&quot;
    }

</code></pre>
<p class="has-line-data" data-line-start="72" data-line-end="73"><strong>Response:</strong></p>
<pre><code class="has-line-data" data-line-start="74" data-line-end="81">    {
        &quot;reponse&quot;: &quot;success&quot;,
        &quot;response_message&quot;: &quot;successfully logged out.&quot;,
        &quot;error_message&quot;: &quot;no error.&quot;
    }

</code></pre>
