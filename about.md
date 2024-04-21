---
title: About me
layout: about
---

<div class="flex flex-col md:flex-row">
    <img src="assets/images/undraw_profile.svg" alt="profile image" class="md:w-1/3">
    <div class="md:pl-8">
        <h1 class="text-5xl font-semibold pt-4 md:pt-0 slide-up">About me.</h1>
        <p class="pt-8 slide-up">As a Backend Developer, I specialize in crafting solutions using the Spring Boot framework in Java, which I deliver seamlessly through Harness, Helm, Docker, Kubernetes, and Openshift. My passion lies in exploring diverse technological stacks for both frontend and backend development, while also staying updated on the latest advancements in Deep Learning. </p>
        <p class="pt-8 slide-up">For any suggestions or improvements please reach out to me over 
        <a class="text-primaryAccent hover:underline" href="{{site.social.linkedin}}">
        LinkedIn</a> or 
        <a class="text-primaryAccent hover:underline" href="{{site.social.github}}">
        GitHub</a>!</p>
    </div>
</div>

<div class="flex flex-col">
    <h1 class="text-5xl font-semibold py-8" id="skill-box">My skills</h1>
    <div class="max-w-4xl">
        <div class="flex flex-col md:flex-row md:flex-wrap md:justify-between">
            {% for skill in site.data.skills %}
                <div class="pt-2 md:pt-0">
                    {{skill.name}}
                    <div class="bg-slate-200 h-6 rounded-md w-64 md:w-96">
                        <div class="to-animate">
                            <div class="bg-primaryAccent text-white
                                text-medium text-right rounded-md h-full" style="width: {{skill.value}}%">
                                <div class="pr-4">{{skill.value}}%</div>
                            </div>
                        </div>
                    </div>
                </div>
            {% endfor %}
        </div>
    </div>
</div>

<div class="flex flex-col pt-12">
    <h1 class="text-5xl font-semibold">Contact</h1>
    <p class="pt-4">If you still need more information about me, please find my resume here.</p>
</div>
