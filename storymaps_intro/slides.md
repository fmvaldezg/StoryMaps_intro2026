---
theme: default
background: ./assets/chair.gif
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## ArcGIS StoryMaps Course
  An introductory course on using ArcGIS StoryMaps
drawings:
  persist: false
transition: slide-left
title: ArcGIS StoryMaps Introduction
mdc: true
---

<style scoped>
.slidev-layout {
  position: relative;
}
.slidev-layout::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-image: inherit;
  background-size: cover;
  background-position: center;
  filter: blur(1px) brightness(0.6);
  z-index: 0;
}
.slidev-layout > * {
  position: relative;
  z-index: 1;
}
</style>

<h1 style="text-shadow: 0 0 20px rgba(0,0,0,0.8), 0 0 40px rgba(0,0,0,0.6), 2px 2px 4px rgba(0,0,0,0.9);">ArcGIS StoryMaps</h1>
<h2 style="text-shadow: 0 0 15px rgba(0,0,0,0.8), 0 0 30px rgba(0,0,0,0.6), 2px 2px 4px rgba(0,0,0,0.9);">Introduction Course</h2>

<p style="text-shadow: 0 0 8px rgba(0,0,0,0.8), 0 0 20px rgba(0,0,0,0.6), 1px 1px 3px rgba(0,0,0,0.9);">Felipe Valdez</p>
<p style="text-shadow: 0 0 8px rgba(0,0,0,0.8), 0 0 20px rgba(0,0,0,0.6), 1px 1px 3px rgba(0,0,0,0.9);">Temple University Libraries</p>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-6 py-3 rounded cursor-pointer text-white font-semibold" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%); box-shadow: 0 4px 15px rgba(0,0,0,0.4);">
    Start Learning →
  </span>
</div>

<img 
  src="https://www.authorsalliance.org/wp-content/uploads/2019/08/Temple_Libraries_Red_Black-e1562689468360-1024x430.png" 
  class="absolute"
  style="left: 5px; top: 310px; width: 170px; background-color: rgba(247, 219, 219, 0.29); padding: 2px; border-radius: 4px;"
  alt="uMap logo"
/>

---
layout: two-cols
---

# Course Menu

Select a chapter to begin learning

::right::

<div class="grid grid-cols-1 gap-2 pr-4 mt-[-1rem]">
  <a @click="$slidev.nav.go(3)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 1: Access StoryMaps</div>
    <div class="text-blue-100 text-xs">Use your tuaccess account</div>
  </a>
  
  <a @click="$slidev.nav.go(4)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 2: Create your first StoryMap</div>
    <div class="text-blue-100 text-xs">Adding a cover, title and  description</div>
  </a>
  
  <a @click="$slidev.nav.go(5)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 3: Adding a Map</div>
    <div class="text-blue-100 text-xs">Incorporating maps, media, and text</div>
  </a>
  
  <a @click="$slidev.nav.go(6)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 4: Adding a Sidecar</div>
    <div class="text-blue-100 text-xs">Immersive experiences</div>
  </a>
  
  <a @click="$slidev.nav.go(7)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 5: Adding a Map Tour</div>
    <div class="text-blue-100 text-xs">Immersive experiences</div>
  </a>
  
  <a @click="$slidev.nav.go(8)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 6: Publishing and sharing</div>
    <div class="text-blue-100 text-xs">Sharing your StoryMap with the world</div>
  </a>
  
  <a @click="$slidev.nav.go(9)" class="block p-2.5 rounded-lg shadow cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
    <div class="text-base font-bold text-white">Chapter 7: Custom design</div>
    <div class="text-blue-100 text-xs">Changing the style of your StoryMap</div>
  </a>
</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);
  background-size: 100%;
  background-clip: text;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=49f486a9-ab7a-4790-9d4c-b3e10140b616&autoplay=false&offerviewer=true&showtitle=false&showbrand=false&captions=true&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 1: Access StoryMaps</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=f363e237-2f67-4252-a3b4-b3e10142923b&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 2: Create your first StoryMap</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=1e132dcd-eedb-4553-96d3-b3e10143f983&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 3: Adding a Map</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=8099454a-3e03-431f-9247-b3e10144baf7&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 4: Adding a Sidecar</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=7d0b2703-1df4-4a65-8841-b3e10145cb45&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 5: Adding a Map Tour</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=2855121b-6bab-4c23-a1ec-b3e10146af1b&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 6: Publishing and sharing</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

---
layout: cover
---

<div class="absolute inset-0 flex flex-col">
  <div class="flex-1 relative">
    <iframe 
      src="https://temple.hosted.panopto.com/Panopto/Pages/Embed.aspx?id=fedb78b0-6193-46a5-a09d-b3e101478465&autoplay=false&offerviewer=true&showtitle=false&showbrand=true&captions=false&interactivity=all" 
      class="absolute inset-0 w-full h-full"
      frameborder="0" 
      allowfullscreen 
      allow="autoplay">
    </iframe>
    <div class="absolute top-4 left-4 bg-black bg-opacity-70 px-4 py-2 rounded">
      <h2 class="text-2xl font-bold text-white">Chapter 7: Custom design</h2>
    </div>
  </div>
  <div class="p-4 text-center bg-gray-900 bg-opacity-80">
    <a @click="$slidev.nav.go(2)" class="px-6 py-2 rounded text-white font-semibold inline-block cursor-pointer transition-all" style="background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);">
      ← Back to Menu
    </a>
  </div>
</div>

--- 
layout: end
---

Need more help:\
[Schedule an appointment here](https://api3.libcal.com/appointments-widget.php?u=106635&iid=1621&t=Make%20an%20Appointment) \
<br>
<br>
Or, email: \
felipe.valdez@temple.edu \
GIS Specialist


<style>
.slidev-layout.end {
  background: linear-gradient(135deg, rgb(164, 30, 53) 0%, rgb(149, 56, 71) 100%);
}
</style>