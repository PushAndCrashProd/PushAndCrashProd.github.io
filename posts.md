---
title: My Posts
layout: posts
---

<div class="flex flex-col p-4 items-center">
    <!-- Parent div for the search bar. -->
    <div class="w-full max-w-5xl h-12 bg-slate-200 rounded-md flex flex-col-reverse items-center md:flex-row">
        <!-- Dropdown to choose between category and content -->
        <div class="w-1/3 max-w-64 bg-white ml-1 p-[6px] rounded-md hover:bg-slate-100 hover:cursor-pointer flex flex-row justify-between">
            <div>Dropdown</div>
            <i data-feather="chevron-down"></i>
        </div>
        <div class="w-full px-2">
            <input class="w-full h-full rounded-md p-[6px] focus:outline-none focus:ring focus:border-primaryAccent" placeholder="Search"/>
        </div>
    </div>
</div>
