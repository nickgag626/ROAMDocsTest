
<!doctype html>
<html>
  <head>
    <meta charset="utf-8">
    <meta content="IE=edge,chrome=1" http-equiv="X-UA-Compatible">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
    <title>Ingenico mPOS SDK Documentation</title>

    <style>
      .highlight table td { padding: 5px; }
.highlight table pre { margin: 0; }
.highlight .gh {
  color: #999999;
}
.highlight .sr {
  color: #f6aa11;
}
.highlight .go {
  color: #888888;
}
.highlight .gp {
  color: #555555;
}
.highlight .gs {
}
.highlight .gu {
  color: #aaaaaa;
}
.highlight .nb {
  color: #f6aa11;
}
.highlight .cm {
  color: #75715e;
}
.highlight .cp {
  color: #75715e;
}
.highlight .c1 {
  color: #75715e;
}
.highlight .cs {
  color: #75715e;
}
.highlight .c, .highlight .cd {
  color: #75715e;
}
.highlight .err {
  color: #960050;
}
.highlight .gr {
  color: #960050;
}
.highlight .gt {
  color: #960050;
}
.highlight .gd {
  color: #49483e;
}
.highlight .gi {
  color: #49483e;
}
.highlight .ge {
  color: #49483e;
}
.highlight .kc {
  color: #66d9ef;
}
.highlight .kd {
  color: #66d9ef;
}
.highlight .kr {
  color: #66d9ef;
}
.highlight .no {
  color: #66d9ef;
}
.highlight .kt {
  color: #66d9ef;
}
.highlight .mf {
  color: #ae81ff;
}
.highlight .mh {
  color: #ae81ff;
}
.highlight .il {
  color: #ae81ff;
}
.highlight .mi {
  color: #ae81ff;
}
.highlight .mo {
  color: #ae81ff;
}
.highlight .m, .highlight .mb, .highlight .mx {
  color: #ae81ff;
}
.highlight .sc {
  color: #ae81ff;
}
.highlight .se {
  color: #ae81ff;
}
.highlight .ss {
  color: #ae81ff;
}
.highlight .sd {
  color: #e6db74;
}
.highlight .s2 {
  color: #e6db74;
}
.highlight .sb {
  color: #e6db74;
}
.highlight .sh {
  color: #e6db74;
}
.highlight .si {
  color: #e6db74;
}
.highlight .sx {
  color: #e6db74;
}
.highlight .s1 {
  color: #e6db74;
}
.highlight .s {
  color: #e6db74;
}
.highlight .na {
  color: #a6e22e;
}
.highlight .nc {
  color: #a6e22e;
}
.highlight .nd {
  color: #a6e22e;
}
.highlight .ne {
  color: #a6e22e;
}
.highlight .nf {
  color: #a6e22e;
}
.highlight .vc {
  color: #ffffff;
}
.highlight .nn {
  color: #ffffff;
}
.highlight .nl {
  color: #ffffff;
}
.highlight .ni {
  color: #ffffff;
}
.highlight .bp {
  color: #ffffff;
}
.highlight .vg {
  color: #ffffff;
}
.highlight .vi {
  color: #ffffff;
}
.highlight .nv {
  color: #ffffff;
}
.highlight .w {
  color: #ffffff;
}
.highlight {
  color: #ffffff;
}
.highlight .n, .highlight .py, .highlight .nx {
  color: #ffffff;
}
.highlight .ow {
  color: #f92672;
}
.highlight .nt {
  color: #f92672;
}
.highlight .k, .highlight .kv {
  color: #f92672;
}
.highlight .kn {
  color: #f92672;
}
.highlight .kp {
  color: #f92672;
}
.highlight .o {
  color: #f92672;
}
    </style>
    <link href="stylesheets/screen.css" rel="stylesheet" media="screen" />
    <link href="stylesheets/print.css" rel="stylesheet" media="print" />
      <script src="javascripts/all.js"></script>
  </head>

  <body class="index" data-languages="[&quot;javascript&quot;,&quot;java&quot;,&quot;swift&quot;]">
    <a href="#" id="nav-button">
      <span>
        NAV
        <img src="images/navbar.png" alt="Navbar" />
      </span>
    </a>
    <div class="toc-wrapper">
      <img src="images/logo.png" class="logo" alt="Logo" />
        <div class="lang-selector">
              <a href="#" data-language-name="javascript">json</a>
              <a href="#" data-language-name="java">Android</a>
              <a href="#" data-language-name="swift">iOS</a>
        </div>
        <div class="search">
          <input type="text" class="search" id="input-search" placeholder="Search">
        </div>
        <ul class="search-results"></ul>
      <div id="toc" class="toc-list-h1">
          <li>
            <a href="#introduction" class="toc-h1 toc-link" data-title="Introduction">Introduction</a>
              <ul class="toc-list-h2">
                  <li>
                    <a href="#prerequisites" class="toc-h2 toc-link" data-title="Introduction">Prerequisites</a>
                  </li>
              </ul>
          </li>
          <li>
            <a href="#wsapi-example-authentication" class="toc-h1 toc-link" data-title="WSAPI Example: Authentication">WSAPI Example: Authentication</a>
              <ul class="toc-list-h2">
                  <li>
                    <a href="#log-in" class="toc-h2 toc-link" data-title="WSAPI Example: Authentication">Log in</a>
                  </li>
                  <li>
                    <a href="#refresh-a-session" class="toc-h2 toc-link" data-title="WSAPI Example: Authentication">Refresh a Session</a>
                  </li>
                  <li>
                    <a href="#logout" class="toc-h2 toc-link" data-title="WSAPI Example: Authentication">Logout</a>
                  </li>
              </ul>
          </li>
          <li>
            <a href="#sdk-example-payment-authorization" class="toc-h1 toc-link" data-title="SDK Example: Payment Authorization">SDK Example: Payment Authorization</a>
              <ul class="toc-list-h2">
                  <li>
                    <a href="#processauthtransactionwithcardreader" class="toc-h2 toc-link" data-title="SDK Example: Payment Authorization">processAuthTransactionWithCardReader</a>
                  </li>
                  <li>
                    <a href="#processkeyedcreditauthtransaction" class="toc-h2 toc-link" data-title="SDK Example: Payment Authorization">processKeyedCreditAuthTransaction</a>
                  </li>
              </ul>
          </li>
          <li>
            <a href="#errors" class="toc-h1 toc-link" data-title="Errors">Errors</a>
          </li>
      </div>
        <ul class="toc-footer">
            <li><a href='#'>Sign Up for a Developer Key</a></li>
            <li><a href='https://www.ingenico.com/our-solutions/mobile-solutions'>Ingenico Mobile Solutions</a></li>
        </ul>
    </div>
    <div class="page-wrapper">
      <div class="dark-box"></div>
      <div class="content">
        <h1 id='introduction'>Introduction</h1>
<p>The Ingenico WSAPI is a set of REST APIs designed to be consumed by API customers for interaction with our Mobile Commerce Manager. This allows customers availability to all of the features that we offer for accepting payments, as well as everything else required for end-end transaction processing</p>
<h2 id='prerequisites'>Prerequisites</h2>
<p>Ingenico uses API keys to allow access to the API. You can register a new API key at our <a href="http://example.com/developers">developer portal</a>.</p>

<aside class="warning">Please replace <code>X-Roam-Key</code> in the header with your API Key.</aside>

<blockquote>
<p>You will receive a session token by logging in</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">Key</span><span class="p">:</span> <span class="s2">"APP6-54a59a59ea7-7440-4f8b-ae96-ffba2e801391"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ApiVersion</span><span class="p">:</span> <span class="s2">"6.0.0"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ClientVersion</span><span class="p">:</span> <span class="s2">"1.0.0"</span>
<span class="nx">Content</span><span class="o">-</span><span class="nx">Type</span><span class="p">:</span> <span class="s2">"application/json"</span>
</code></pre><h3 id='headers'>Headers</h3>
<table><thead>
<tr>
<th>Parameter</th>
<th>Required</th>
<th>Description</th>
</tr>
</thead><tbody>
<tr>
<td>X-Roam-Key</td>
<td>Yes</td>
<td>Application token that identifies the request origin. This key is unique to every client, as well as every environment. Please contact API Support (APIsupport.us@ingenico.com) to get this key.</td>
</tr>
<tr>
<td>X-Roam-ApiVersion</td>
<td>Yes</td>
<td>Version of the API being used (e.g. 6.0.0)</td>
</tr>
<tr>
<td>X-Roam-ClientVersion</td>
<td>Yes</td>
<td>Client version which can be vary by application. This is set by developers (e.g. 1.0.0)</td>
</tr>
<tr>
<td>Content-Type</td>
<td>Yes</td>
<td>Content type e.g. application/json</td>
</tr>
</tbody></table>
<h1 id='wsapi-example-authentication'>WSAPI Example: Authentication</h1><h2 id='log-in'>Log in</h2>
<blockquote>
<p>Header</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">Key</span><span class="p">:</span> <span class="s2">"APP6-54a59a59ea7-7440-4f8b-ae96-ffba2e801391"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ApiVersion</span><span class="p">:</span> <span class="s2">"6.0.0"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ClientVersion</span><span class="p">:</span> <span class="s2">"1.0.0"</span>
<span class="nx">Content</span><span class="o">-</span><span class="nx">Type</span><span class="p">:</span> <span class="s2">"application/json"</span>

</code></pre>
<blockquote>
<p>Request</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="p">{</span>
  <span class="s2">"user_name"</span><span class="p">:</span><span class="s2">"myUserName"</span><span class="p">,</span>
  <span class="s2">"password"</span><span class="p">:</span><span class="s2">"pwd123"</span>
<span class="p">}</span>

</code></pre>
<blockquote>
<p>The above command returns JSON structured like this:</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="p">{</span>
  <span class="s2">"chain_id"</span><span class="p">:</span> <span class="s2">"679"</span><span class="p">,</span>
  <span class="s2">"store_id"</span><span class="p">:</span> <span class="s2">"3"</span><span class="p">,</span>
  <span class="s2">"terminal_id"</span><span class="p">:</span> <span class="s2">"1"</span><span class="p">,</span>
  <span class="s2">"organization_id"</span><span class="p">:</span> <span class="s2">"8"</span><span class="p">,</span>
  <span class="s2">"organization_type"</span><span class="p">:</span> <span class="s2">"merchant"</span><span class="p">,</span>
  <span class="s2">"processor"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"name"</span><span class="p">:</span> <span class="s2">"Vantiv"</span><span class="p">,</span>
    <span class="s2">"processor_profile"</span><span class="p">:</span> <span class="s2">"vantiv_profile1"</span><span class="p">,</span>
    <span class="s2">"date_modified"</span><span class="p">:</span> <span class="s2">"20151113190112"</span>
  <span class="p">},</span>
  <span class="s2">"session"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"expires"</span><span class="p">:</span> <span class="s2">"20151222175141"</span><span class="p">,</span>
    <span class="s2">"session_token"</span><span class="p">:</span> <span class="s2">"MCM6-fd55c7-7429-447c-9918-c80162574cdb"</span>
  <span class="p">},</span>
  <span class="s2">"user"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"user_name"</span><span class="p">:</span> <span class="s2">"myUserName"</span><span class="p">,</span>
    <span class="s2">"bill_organization"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"is_admin"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"is_sys_admin"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"account_flags"</span><span class="p">:</span> <span class="p">{</span>
      <span class="s2">"change_email_required"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
      <span class="s2">"change_password_required"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
      <span class="s2">"change_security_questions_required"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
      <span class="s2">"accept_terms_and_conditions_required"</span><span class="p">:</span> <span class="kc">false</span>
    <span class="p">},</span>
    <span class="s2">"primary_email"</span><span class="p">:</span> <span class="s2">"myEmail@ingenico.com"</span><span class="p">,</span>
    <span class="s2">"security_questions"</span><span class="p">:</span> <span class="p">[</span>
      <span class="p">{</span>
        <span class="s2">"answer"</span><span class="p">:</span> <span class="s2">"testAnswer"</span><span class="p">,</span>
        <span class="s2">"id"</span><span class="p">:</span> <span class="s2">"13"</span><span class="p">,</span>
        <span class="s2">"question"</span><span class="p">:</span> <span class="s2">"What is the name of your favorite childhood friend?"</span>
      <span class="p">},</span>
      <span class="p">{</span>
        <span class="s2">"answer"</span><span class="p">:</span> <span class="s2">"testAnswer"</span><span class="p">,</span>
        <span class="s2">"id"</span><span class="p">:</span> <span class="s2">"15"</span><span class="p">,</span>
        <span class="s2">"question"</span><span class="p">:</span> <span class="s2">"What school did you attend for sixth grade?"</span>
      <span class="p">}</span>
    <span class="p">],</span>
    <span class="s2">"cell_phone"</span><span class="p">:</span> <span class="s2">"1151151155"</span><span class="p">,</span>
    <span class="s2">"first_name"</span><span class="p">:</span> <span class="s2">"MyFirstName"</span><span class="p">,</span>
    <span class="s2">"last_name"</span><span class="p">:</span> <span class="s2">"MyLastName"</span><span class="p">,</span>
    <span class="s2">"locale"</span><span class="p">:</span> <span class="s2">"en-US"</span><span class="p">,</span>
    <span class="s2">"middle_name_initial"</span><span class="p">:</span> <span class="s2">""</span><span class="p">,</span>
    <span class="s2">"other_phone"</span><span class="p">:</span> <span class="s2">""</span><span class="p">,</span>
    <span class="s2">"test_account"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"title"</span><span class="p">:</span> <span class="s2">""</span><span class="p">,</span>
    <span class="s2">"work_phone"</span><span class="p">:</span> <span class="s2">"1001001000"</span>
  <span class="p">},</span>
  <span class="s2">"configuration"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"account.locale.available_locales"</span><span class="p">:</span> <span class="s2">"en_US, en_CA"</span><span class="p">,</span>
    <span class="s2">"account.permissions.add_submerchant.merchant_portal"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"account.permissions.allow_submerchants"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"account.permissions.change_address"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"account.permissions.change_name"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"account.permissions.edit_email_receipt"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"account.permissions.order_accessories.merchant_portal"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"branding.theme"</span><span class="p">:</span> <span class="s2">"default"</span><span class="p">,</span>
    <span class="s2">"branding.theme.available_themes"</span><span class="p">:</span> <span class="s2">"default"</span><span class="p">,</span>
    <span class="s2">"component.access.inventory_management"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"component.access.virtual_terminal"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.avs"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.avs.reverse_mismatch"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"processing.config.capture_signature"</span><span class="p">:</span> <span class="s2">"Optional"</span><span class="p">,</span>
    <span class="s2">"processing.config.collect_geolocation"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.collect_optional_info"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.processor_profile"</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span>
    <span class="s2">"processing.config.currency"</span><span class="p">:</span> <span class="p">{</span>
      <span class="s2">"code"</span><span class="p">:</span> <span class="s2">"USD"</span><span class="p">,</span>
      <span class="s2">"iso"</span><span class="p">:</span> <span class="mi">840</span><span class="p">,</span>
      <span class="s2">"symbol"</span><span class="p">:</span> <span class="s2">"$"</span>
    <span class="p">},</span>
    <span class="s2">"processing.config.cvv"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.cvv.reverse_mismatch"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"processing.config.discount"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.show_paper_receipt"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.small_ticket"</span><span class="p">:</span> <span class="s2">"Off"</span><span class="p">,</span>
    <span class="s2">"processing.config.small_ticket.contactless"</span><span class="p">:</span> <span class="s2">"Off"</span><span class="p">,</span>
    <span class="s2">"processing.config.small_ticket.contactless.max"</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
    <span class="s2">"processing.config.small_ticket.max"</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
    <span class="s2">"processing.config.tax"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.config.tax.default"</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span>
    <span class="s2">"processing.config.tender_types"</span><span class="p">:</span> <span class="p">[</span>
      <span class="s2">"Cash"</span><span class="p">,</span>
      <span class="s2">"Card"</span>
    <span class="p">],</span>
    <span class="s2">"processing.config.tip"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.manual_entry"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.refund"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.refund.for_submerchant"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.refund.merchant_portal"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.refund.mobile"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.refund.smart_refund"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.permissions.void"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"processing.receipt.show_tax"</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
    <span class="s2">"security.session_timeout.mobile"</span><span class="p">:</span> <span class="mi">15</span><span class="p">,</span>
    <span class="s2">"security.account_locking.count_memory"</span><span class="p">:</span> <span class="s2">"30"</span><span class="p">,</span>
    <span class="s2">"security.account_locking.failed_attempts_limit"</span><span class="p">:</span> <span class="mi">3</span><span class="p">,</span>
    <span class="s2">"security.account_locking.lockout_duration"</span><span class="p">:</span> <span class="mi">2</span>
  <span class="p">}</span>
<span class="p">}</span>

</code></pre>
<p>This call will log in to the system and return a session token, along with various user settings.</p>
<h3 id='http-request'>HTTP Request</h3>
<p><code>POST http://example.com/WSAPI/Authentication</code></p>
<h3 id='query-parameters'>Query Parameters</h3>
<table><thead>
<tr>
<th>Parameter</th>
<th>Required</th>
<th>Description</th>
</tr>
</thead><tbody>
<tr>
<td>user_name</td>
<td>Yes</td>
<td>User name</td>
</tr>
<tr>
<td>password</td>
<td>Yes</td>
<td>Password</td>
</tr>
</tbody></table>
<h3 id='response-parameters'>Response Parameters</h3>
<table><thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead><tbody>
<tr>
<td>chainID</td>
<td>String</td>
<td>xxx</td>
</tr>
<tr>
<td>store_id</td>
<td>String</td>
<td>xxx</td>
</tr>
<tr>
<td>terminal_id</td>
<td>String</td>
<td>xxx</td>
</tr>
<tr>
<td>organization_id</td>
<td>String</td>
<td>xxx</td>
</tr>
<tr>
<td>organization_type</td>
<td>OrganizationType</td>
<td>xxx</td>
</tr>
<tr>
<td>processor</td>
<td>Processor</td>
<td>xxx</td>
</tr>
<tr>
<td>session</td>
<td>Session</td>
<td>xxx</td>
</tr>
<tr>
<td>user</td>
<td>user</td>
<td>xxx</td>
</tr>
<tr>
<td>configuration</td>
<td>List</td>
<td>xxx</td>
</tr>
</tbody></table>

<aside class="success">
Remember — This will return your session token!
</aside>
<h2 id='refresh-a-session'>Refresh a Session</h2>
<blockquote>
<p>Header</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">Token</span><span class="p">:</span> <span class="s2">"MCM6-420ba742-ee06-401a-b1a6-0f6054a3e20d"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ApiVersion</span><span class="p">:</span> <span class="s2">"6.0.0"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ClientVersion</span><span class="p">:</span> <span class="s2">"1.0.0"</span>
<span class="nx">Content</span><span class="o">-</span><span class="nx">Type</span><span class="p">:</span> <span class="s2">"application/json"</span>
</code></pre>
<blockquote>
<p>Request</p>
</blockquote>
<pre class="highlight json tab-json"><code><span class="w">

</span></code></pre>
<blockquote>
<p>The above command returns JSON structured like this:</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="p">{</span>
  <span class="s2">"chain_id"</span><span class="p">:</span> <span class="s2">"679"</span><span class="p">,</span>
  <span class="s2">"store_id"</span><span class="p">:</span> <span class="s2">"3"</span><span class="p">,</span>
  <span class="s2">"terminal_id"</span><span class="p">:</span> <span class="s2">"1"</span><span class="p">,</span>
  <span class="s2">"organization_type"</span><span class="p">:</span> <span class="s2">"merchant"</span><span class="p">,</span>
  <span class="s2">"session"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"expires"</span><span class="p">:</span> <span class="s2">"20151222175141"</span><span class="p">,</span>
    <span class="s2">"session_token"</span><span class="p">:</span> <span class="s2">"MCM6-420ba742-ee06-401a-b1a6-0f6054a3e20d"</span>
  <span class="p">},</span>
  <span class="s2">"user"</span><span class="p">:</span> <span class="p">{</span>
    <span class="s2">"user_name"</span><span class="p">:</span> <span class="s2">"myUserName"</span><span class="p">,</span>
    <span class="s2">"is_admin"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"is_sys_admin"</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
    <span class="s2">"test_account"</span><span class="p">:</span> <span class="kc">false</span>
  <span class="p">}</span>
<span class="p">}</span>

</code></pre>
<aside class="notice">Please replace <code>X-Roam-Token</code> (in the header) with your session token returned from Login.</aside>

<p>Keeps the logged in session alive. This API method refreshes a valid session and extends the session token expiry time. </p>
<h3 id='http-request-2'>HTTP Request</h3>
<p><code>PUT http://example.com/WSAPI/Authentication</code></p>
<h3 id='query-parameters-2'>Query Parameters</h3>
<table><thead>
<tr>
<th>Parameter</th>
<th>Description</th>
</tr>
</thead><tbody>
<tr>
<td>NA</td>
<td>NA</td>
</tr>
</tbody></table>

<aside class="success">HTTP Status code: 200 OK denotes success</aside>
<h2 id='logout'>Logout</h2>
<blockquote>
<p>Header</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">Token</span><span class="p">:</span> <span class="s2">"MCM6-420ba742-ee06-401a-b1a6-0f6054a3e20d"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ApiVersion</span><span class="p">:</span> <span class="s2">"6.0.0"</span>
<span class="nx">X</span><span class="o">-</span><span class="nx">Roam</span><span class="o">-</span><span class="nx">ClientVersion</span><span class="p">:</span> <span class="s2">"1.0.0"</span>
<span class="nx">Content</span><span class="o">-</span><span class="nx">Type</span><span class="p">:</span> <span class="s2">"application/json"</span>
</code></pre>
<blockquote>
<p>Request</p>
</blockquote>
<pre class="highlight json tab-json"><code><span class="w">
</span></code></pre>
<blockquote>
<p>The above command returns this response:</p>
</blockquote>
<pre class="highlight javascript tab-javascript"><code><span class="nx">HTTP</span> <span class="nx">Status</span> <span class="nx">Code</span> <span class="mi">200</span> <span class="nx">OK</span>

</code></pre>
<p>This call will log the user out of an active session, invalidating the existing session token.</p>
<h3 id='http-request-3'>HTTP Request</h3>
<p><code>DELETE http://example.com/WSAPI/Authentication</code></p>
<h3 id='url-parameters'>URL Parameters</h3>
<table><thead>
<tr>
<th>Parameter</th>
<th>Description</th>
</tr>
</thead><tbody>
<tr>
<td>NA</td>
<td>NA</td>
</tr>
</tbody></table>

<aside class="success">HTTP Status code: 200 OK denotes success</aside>
<h1 id='sdk-example-payment-authorization'>SDK Example: Payment Authorization</h1><h2 id='processauthtransactionwithcardreader'>processAuthTransactionWithCardReader</h2><pre class="highlight java tab-java"><code><span class="n">CreditAuthTransactionRequest</span> <span class="n">request</span> <span class="o">=</span> <span class="k">new</span> <span class="n">CreditAuthTransactionRequest</span><span class="o">(</span><span class="n">amount</span><span class="o">,</span>
<span class="n">productList</span><span class="o">,</span> <span class="n">longitude</span><span class="o">,</span> <span class="n">latitude</span><span class="o">,</span>
<span class="n">transactionGroupID</span><span class="o">);</span>

<span class="n">Ingenico</span><span class="o">.</span><span class="na">getInstance</span><span class="o">().</span><span class="na">payment</span><span class="o">().</span><span class="na">processAuthTransactionWithCardReader</span><span class="o">(</span><span class="n">request</span>
<span class="o">,</span> <span class="k">new</span> <span class="n">TransactionCallbackImpl</span><span class="o">());</span>

</code></pre><pre class="highlight swift tab-swift"><code><span class="kt">IMSCreditAuthTransactionRequest</span> <span class="o">*</span><span class="n">request</span> <span class="o">=</span> <span class="p">[[</span><span class="kt">IMSCreditAuthTransactionRequest</span> <span class="n">alloc</span><span class="p">]</span> <span class="nv">initWithAmount</span><span class="p">:</span><span class="n">amount</span>
                                                                                       <span class="nv">andProducts</span><span class="p">:</span><span class="n">productList</span>                                                                                 
                                                                                      <span class="nv">andLongitude</span><span class="p">:</span><span class="n">longitude</span>
                                                                                       <span class="nv">andLatitude</span><span class="p">:</span><span class="n">latitude</span>
                                                                             <span class="nv">andTransactionGroupID</span><span class="p">:</span><span class="n">transactionGroupID</span>
                                                                               <span class="nv">andTransactionNotes</span><span class="p">:</span><span class="n">transactionNote</span>
                                                                              <span class="nv">andMerchantInvoiceID</span><span class="p">:</span><span class="n">invocieID</span>
                                                                   <span class="nv">andShowNotesAndInvoiceOnReceipt</span><span class="p">:</span><span class="kc">true</span>
                                                                         <span class="nv">andTokenRequestParameters</span><span class="p">:</span><span class="n">tokenRequest</span><span class="p">];</span>


<span class="p">[[</span><span class="kt">Ingenico</span> <span class="n">sharedInstance</span><span class="p">]</span><span class="o">.</span><span class="kt">Payment</span> <span class="nv">processCreditAuthTransactionWithCardReader</span><span class="p">:</span><span class="n">request</span>
                               <span class="nv">andUpdateProgress</span><span class="p">:</span><span class="o">^</span><span class="p">(</span><span class="kt">IMSProgressMessage</span> <span class="n">message</span><span class="p">,</span> <span class="kt">NSString</span> <span class="o">*</span><span class="n">extraMessage</span><span class="p">)</span>
                               <span class="p">{</span>
                                    <span class="cm">/*The progress message indicates the stage the transaction is at*/</span>
                               <span class="p">}</span>
                               <span class="nv">andSelectApplication</span><span class="p">:</span><span class="o">^</span><span class="p">(</span><span class="kt">NSArray</span> <span class="o">*</span><span class="n">applicationList</span><span class="p">,</span> <span class="kt">NSError</span> <span class="o">*</span><span class="n">error</span><span class="p">,</span> <span class="kt">ApplicationSelectedResponse</span> <span class="o">*</span><span class="n">appReponse</span><span class="p">)</span>
                               <span class="p">{</span>
                                    <span class="cm">/*This callback indicates the card inserted supports multiple Applications and requires user to pick one for this transaction*/</span>
                               <span class="p">}</span>
                               <span class="nv">andOnDone</span><span class="p">:</span><span class="o">^</span><span class="p">(</span><span class="kt">IMSTransactionResponse</span> <span class="o">*</span><span class="n">response</span><span class="p">,</span> <span class="kt">NSError</span> <span class="o">*</span><span class="n">error</span><span class="p">)</span>
                               <span class="p">{</span>
                                    <span class="k">if</span><span class="p">(</span><span class="o">!</span><span class="n">error</span><span class="p">){</span>
                                        <span class="cm">/*Transaction succeeded(code in the response will indicates the result of the transaction)*/</span>
                                    <span class="p">}</span>
                                    <span class="k">else</span><span class="p">{</span>
                                        <span class="cm">/*Transaction failed and the responseCode will indicate the error */</span>
                                        <span class="kt">NSInteger</span> <span class="n">responseCode</span> <span class="o">=</span> <span class="n">error</span><span class="o">.</span><span class="n">code</span><span class="p">;</span>
                                    <span class="p">}</span>
                               <span class="p">}];</span>


</code></pre><h3 id='description'>Description</h3>
<p>In order to use the SDK, you will first need to initialize it, login, and setup the card reader. This is done to validate a user’s authenticity to use the application, and begin working with the SDK. Please refer to the Ingenico mPOS SDK User Guide (Section 4) if you need assistance with this. 
One properly initialized and setup, this method call can be used to process a pre-authorized transaction. This will temporarily place the funds on hold, which can then be completed or voided if necessary. </p>
<h3 id='required-objects'>Required Objects</h3>
<table><thead>
<tr>
<th>Object Name</th>
<th>Object Type</th>
<th>Decription</th>
</tr>
</thead><tbody>
<tr>
<td>amount</td>
<td>Amount</td>
<td>Cost of the sale</td>
</tr>
<tr>
<td>products</td>
<td>List<Product></td>
<td>List of the products</td>
</tr>
<tr>
<td>longitude</td>
<td>String</td>
<td>The location&#39;s longitude</td>
</tr>
<tr>
<td>latitude</td>
<td>String</td>
<td>The location&#39;s latitude</td>
</tr>
<tr>
<td>transactionGroupID</td>
<td>String</td>
<td>TBI - set as null</td>
</tr>
</tbody></table>
<h2 id='processkeyedcreditauthtransaction'>processKeyedCreditAuthTransaction</h2><pre class="highlight java tab-java"><code><span class="n">KeyedCreditAuthTransactionRequest</span> <span class="n">request</span> <span class="o">=</span> <span class="k">new</span> <span class="n">KeyedCreditAuthTransactionRequest</span><span class="o">(</span><span class="n">card</span><span class="o">,</span>
                                                                                    <span class="n">saleAmount</span><span class="o">,</span>
                                                                                    <span class="n">products</span><span class="o">,</span>
                                                                                    <span class="n">clerkID</span><span class="o">,</span>
                                                                                    <span class="n">longitude</span><span class="o">,</span>
                                                                                    <span class="n">latitude</span><span class="o">,</span>
                                                                                    <span class="kc">null</span><span class="o">,</span>
                                                                                    <span class="n">transactionNote</span><span class="o">,</span>
                                                                                    <span class="n">merchantInvocieID</span><span class="o">,</span>
                                                                                    <span class="n">Boolean</span><span class="o">.</span><span class="na">TRUE</span><span class="o">,</span>  <span class="c1">//showNotesAndInvoiceOnReceipt</span>
                                                                                    <span class="n">tokenRequest</span><span class="o">);</span>
<span class="n">Ingenico</span><span class="o">.</span><span class="na">getInstance</span><span class="o">().</span><span class="na">payment</span><span class="o">().</span><span class="na">processKeyedCreditAuthTransaction</span><span class="o">(</span><span class="n">request</span><span class="o">,</span><span class="k">new</span> <span class="n">TransactionCallbackImpl</span><span class="o">());</span>


</code></pre><pre class="highlight swift tab-swift"><code>
<span class="kt">IMSKeyedCreditAuthTransactionRequest</span> <span class="o">*</span><span class="n">request</span> <span class="o">=</span> <span class="p">[[</span><span class="kt">IMSKeyedCreditAuthTransactionRequest</span> <span class="n">alloc</span><span class="p">]</span> <span class="nv">initWithCard</span><span class="p">:</span><span class="n">card</span>
                                                                        <span class="nv">andAmount</span><span class="p">:</span><span class="n">amount</span>
                                                                      <span class="nv">andProducts</span><span class="p">:</span><span class="n">products</span>
                                                                       <span class="nv">andClerkID</span><span class="p">:</span><span class="n">clerkID</span>
                                                                     <span class="nv">andLongitude</span><span class="p">:</span><span class="n">longitude</span>
                                                                      <span class="nv">andLatitude</span><span class="p">:</span><span class="n">latitude</span>
                                                            <span class="nv">andTransactionGroupID</span><span class="p">:</span><span class="kc">nil</span>
                                                              <span class="nv">andTransactionNotes</span><span class="p">:</span><span class="n">transactionNote</span>
                                                             <span class="nv">andMerchantInvoiceID</span><span class="p">:</span><span class="n">invocieID</span>
                                                  <span class="nv">andShowNotesAndInvoiceOnReceipt</span><span class="p">:</span><span class="kc">true</span>
                                                        <span class="nv">andTokenRequestParameters</span><span class="p">:</span><span class="n">tokenRequest</span><span class="p">];</span>

<span class="p">[[</span><span class="kt">Ingenico</span> <span class="n">sharedInstance</span><span class="p">]</span><span class="o">.</span><span class="kt">Payment</span> <span class="nv">processKeyedCreditAuthTransaction</span><span class="p">:</span><span class="n">request</span>
                               <span class="nv">andOnDone</span><span class="p">:</span><span class="o">^</span><span class="p">(</span><span class="kt">IMSTransactionResponse</span> <span class="o">*</span><span class="n">response</span><span class="p">,</span> <span class="kt">NSError</span> <span class="o">*</span><span class="n">error</span><span class="p">)</span>
                               <span class="p">{</span>
                                    <span class="k">if</span><span class="p">(</span><span class="o">!</span><span class="n">error</span><span class="p">){</span>
                                        <span class="cm">/*Transaction succeeded(code in the response will indicates the result of the transaction)*/</span>
                                    <span class="p">}</span>
                                    <span class="k">else</span><span class="p">{</span>
                                        <span class="cm">/*Transaction failed and the responseCode will indicate the error */</span>
                                        <span class="kt">NSInteger</span> <span class="n">responseCode</span> <span class="o">=</span> <span class="n">error</span><span class="o">.</span><span class="n">code</span><span class="p">;</span>
                                    <span class="p">}</span>
                               <span class="p">}];</span>


</code></pre><h3 id='description-2'>Description</h3>
<p>Similar to processing a transaction with the card reader (Section 2_1), you must first initialize the SDK and login before processing a transaction.<br>
This section describes how to process a pre-authorization transaction by manually keying in the card information to include:</p>

<ul>
<li>Credit Card Number</li>
<li>Expiration Date</li>
<li>CVV2/CVC Code</li>
</ul>

<p>The method in which you input the above information is completely up to you. The most common way is to have an on-screen number pad to type in the numbers. Processing credit cards manually is also an optional functionality for your application. </p>

<p><strong>If you do not plan on allowing your merchants to accept payment by manually entering a card number, you can disregard this section.</strong>**</p>

<p>Again, this will temporarily place the funds on hold, which can then be completed or voided if necessary.</p>
<h3 id='required-objects-2'>Required Objects</h3>
<table><thead>
<tr>
<th>Object Name</th>
<th>Object Type</th>
<th>Decription</th>
</tr>
</thead><tbody>
<tr>
<td>card</td>
<td>Card</td>
<td>Credit Card Information</td>
</tr>
<tr>
<td>amount</td>
<td>Amount</td>
<td>Cost of the sale</td>
</tr>
<tr>
<td>products</td>
<td>List<Product></td>
<td>List of the products</td>
</tr>
<tr>
<td>clerkID</td>
<td>String</td>
<td>Key identifying the client</td>
</tr>
<tr>
<td>longitude</td>
<td>String</td>
<td>The location&#39;s longitude</td>
</tr>
<tr>
<td>latitude</td>
<td>String</td>
<td>The location&#39;s latitude</td>
</tr>
</tbody></table>
<h1 id='errors'>Errors</h1>
<aside class="notice">This error section is stored in a separate file in `includes/_errors.md`. Slate allows you to optionally separate out your docs into many files...just save them to the `includes` folder and add them to the top of your `index.md`'s frontmatter. Files are included in the order listed.</aside>

<p>The Kittn API uses the following error codes:</p>

<table><thead>
<tr>
<th>Error Code</th>
<th>Meaning</th>
</tr>
</thead><tbody>
<tr>
<td>400</td>
<td>Bad Request -- Your request is invalid.</td>
</tr>
<tr>
<td>401</td>
<td>Unauthorized -- Your API key is wrong.</td>
</tr>
<tr>
<td>403</td>
<td>Forbidden -- The call requested is hidden for administrators only.</td>
</tr>
<tr>
<td>404</td>
<td>Not Found -- The specified request could not be found.</td>
</tr>
<tr>
<td>405</td>
<td>Method Not Allowed -- You tried to access an invalid method.</td>
</tr>
<tr>
<td>406</td>
<td>Not Acceptable -- You requested a format that isn&#39;t json.</td>
</tr>
<tr>
<td>410</td>
<td>Gone -- The API requested has been removed from our servers.</td>
</tr>
<tr>
<td>500</td>
<td>Internal Server Error -- We had a problem with our server. Try again later.</td>
</tr>
<tr>
<td>503</td>
<td>Service Unavailable -- We&#39;re temporarily offline for maintenance. Please try again later.</td>
</tr>
</tbody></table>

      </div>
      <div class="dark-box">
          <div class="lang-selector">
                <a href="#" data-language-name="javascript">json</a>
                <a href="#" data-language-name="java">Android</a>
                <a href="#" data-language-name="swift">iOS</a>
          </div>
      </div>
    </div>
  </body>
</html>