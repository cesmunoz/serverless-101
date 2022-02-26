---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://sm-services.es/wp-content/uploads/2020/10/Serverless-computing-o-funciones-lambda-img.jpg
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

# Intro to Serverless

Serverless 101 con CemDev

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/cesmunoz/" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# ⚡ What is Serverless?

<br>
<br>

- ⚡ **No server** - sort of ... there will be server. but on the cloud
- ⚡ **Cloud-Base Development** - sets developers free to focus on only writing code to solve business problems instead of managing server issues
- ⚡ **Auto scaling** - The power you need to execute applications are allocated on demand

<br>
<br>

In other words...Serverless is awesome!!

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# ⚡ Benefits of Serverless

<br>
<br>

- ⚡ **Picking operating systems** - No more!
- ⚡ **Configuring networking** - No more! 
- ⚡ **Path Dependencies** - No more...well we still have dependencies with npm, right?
- ⚡ **Patch capacity** - No more!
- ⚡ **Cost** - No mo...wait, yes, you will paid. Nothing is cheap you know? But the cost is really low
- ⚡ **Separations of concerns** - You can develop and test each functionality septate for each other.


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# ⚡ What we can do on serverless?

<br>
<br>
Well...whatever we want the same thing that we can do on a server
<br>

- ⚡ **Call from a API**
- ⚡ **Send Emails**
- ⚡ **Push Notifications**
- ⚡ **Run Cron Jobs**
- ⚡ **Trigger by an Event Queue / Streams**
- ⚡ **IoT Devices**

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# ⚡ Examples

Example 1
<img
  v-click
  class="absolute left-15 w-60"
  src="https://fractel.com/wp-content/uploads/2019/01/Cloud_Icon-01.png"
/>
<img
  v-after
  v-click
  class="absolute left-100 w-60"
  src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8f/Orange_lambda.svg/1959px-Orange_lambda.svg.png"
/>
<img
  v-after
  v-click
  class="absolute left-180 w-60"
  src="https://www.eximoproject.pl/images/ico-base.png"
/>

---

# ⚡ Examples

Example 2
<img
  v-click
  class="absolute left-15 w-60"
  src="https://icon-library.com/images/scheduler-icon/scheduler-icon-5.jpg"
/>
<img
  v-after
  v-click
  class="absolute left-100 w-60"
  src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8f/Orange_lambda.svg/1959px-Orange_lambda.svg.png"
/>
<img
  v-after
  v-click
  class="absolute left-180 w-60"
  src="https://www.freepnglogos.com/uploads/email-png/blue-email-box-circle-png-transparent-icon-2.png"
/>

---

# ⚡ Where I can use Serverless Functions?

Almost anywhere

- ⚡ **AWS** - Lambda Functions (we are going to work here)
- ⚡ **Google Cloud Functions**
- ⚡ **Azure Functions**
- ⚡ **Vercel Functions**
- ⚡ **Netlify Functions**


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---


# ⚡ Not everything is good in the serverless world

The cons

- ⚡ **Cold Start**
- ⚡ **Challenging for Debug**
- ⚡ **Complexity**
- ⚡ **Limitation of runnings**
- ⚡ **Vercel Functions**
- ⚡ **Netlify Functions**


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# ⚡ DEMO TIME

<img
  class="absolute left-15 w-200"
  src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"
/>


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


---

<img
  class="absolute left-50 w-150"
  src="https://media.giphy.com/media/d68IdpvmAHohx5NMEV/giphy.gif"
/>
