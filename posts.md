---
title: My Posts
layout: posts
---

<div class="flex flex-col">
    <!-- Search box   -->
    <div class="flex flex-row p-4 justify-center items-center">
        <input 
            placeholder="Search by title or keywords"  
            class="w-full md:w-3/5 p-3 rounded-lg"
            onkeyup="processPosts(this)"/>
        <i class="bg-primaryAccent text-white p-1 w-8 h-8 rounded-xl -ml-9" data-feather="search"></i>
    </div>
    <div class="flex flex-row-reverse justify-evenly items-center flex-wrap-reverse gap-4 py-8" id="posts-area">
        <!-- Have all the posts visible at the start -->
        {% for post in site.posts %}
            <a class="outline:none" href="{{post.url}}">
                <div class="max-w-sm rounded overflow-hidden shadow-lg transition-colors hover:bg-primaryAccent hover:text-white">
                    <div class="px-6 py-4">
                        <div class="font-bold text-xl mb-2">{{post.title}}</div>
                        <p class="text-base">
                        {{post.excerpt}}
                        </p>
                        <div class="pt-4 font-extralight">
                            <em>by {{post.author}} on {{ post.date | date: '%e %B %Y' }}</em>
                        </div>
                    </div>
                    <div class="px-6 pt-4 pb-2">
                        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{{post.keyword1}}</span>
                        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{{post.keyword2}}</span>
                        <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{{post.keyword3}}</span>
                    </div>
                </div>
            </a>
        {% endfor %}
    </div>

</div>
