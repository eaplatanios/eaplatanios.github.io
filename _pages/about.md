---
layout: page
permalink: /
title: about
nav: about
---

<div class="text-center mt-5">
  <img class="profile-img" src="{{ 'prof_pic.jpg' | prepend: '/assets/img/' | prepend: site.baseurl }}">
</div>

<div class="col mt-4">
  <h1 class="title text-center font-weight-bold">Anthony Platanios</h1>
  <div class="row mt-3 mb-3">
    <div class="col">
      <h6 class="mt-1 text-center text-sm-center" style="font-stretch: ultra-condensed;">
        VP of Research<br/>
        <a href="https://www.scaledcognition.com/">Scaled Cognition</a>
      </h6>
    </div>
    <!-- <div class="col-sm-6">
      <h6 class="mt-1 text-left text-sm-right" style="font-stretch: ultra-condensed;">
        <a style="color: rgb(60, 72, 88);" href="http://www.ml.cmu.edu/" target="_blank">Principal Researcher</a><br/>
        <a style="color: rgb(60, 72, 88);" href="http://www.cs.cmu.edu/" target="_blank">Semantic Machines</a><br/>
        <a style="color: rgb(60, 72, 88);" href="http://www.cmu.edu/" target="_blank">Microsoft</a>
      </h6>
    </div>
    <div class="col-sm-6">
      <h6 class="mt-1 text-left text-sm-left" style="font-stretch: ultra-condensed;">
        Berkeley Way West, Floor 7<br/>
        1919 Shattuck Ave<br/>
        Berkeley, CA, 94704
      </h6>
    </div> -->
  </div>
</div>

<!-- Introduction -->

<div class="col text-justify p-0">
  I am the VP of Research at <a href="https://www.scaledcognition.com/">Scaled Cognition</a> and a member of the founding team, where we are developing the next generation of LLMs for agentic use cases, which are reliable, offer certain classes of hard guarantees on their behavior, and do not hallucinate.
  <br/><br/>
  Previously, I was a Senior Principal Researcher at <a href="https://www.microsoft.com/en-us/research/project/semantic-machines/" target="_blank">Microsoft Semantic Machines</a>, where I led the design and development of a system that aims to predict the next user action (e.g., sending an email, opening a file, adding specific people to a calendar invite, etc.) based on what a user and others in their network have been doing (underlying this system was a novel Foundation Model over user actions). I managed a team across both research and engineering, and helped set the technical direction for the broader organization. I invested heavily in aligning research and engineering, and I worked closely with multiple partner teams at Microsoft to deliver on our objectives, while also helping improve the underlying platform and infrastructure that we leveraged. Earlier on in my career at Microsoft I also served as a key contributor to the research and development of the Semantic Machines conversational AI platform which handled user requests by using a neural network to synthesize computer programs in a new proprietary programming language. I designed and shipped the program synthesis neural network (i.e., a contextual semantic parser) that powers the platform.
  <br/><br/>
  Prior to that, I was a PhD student in the <a href="http://www.ml.cmu.edu/" target="_blank">Machine Learning Department</a> of the <a href="https://www.scs.cmu.edu/" target="_blank">School of Computer Science</a> at <a href="http://www.cmu.edu/" target="_blank">Carnegie Mellon University</a>. My advisor was <a href="http://www.cs.cmu.edu/~tom/" target="_blank">Tom Mitchell</a> and I worked on <a href="http://rtw.ml.cmu.edu/rtw/" target="_blank">Never-Ending Learning</a>. My PhD thesis on learning collections of functions can be found <a href="{{ '/assets/pdf/thesis/thesis.pdf' | prepend: site.baseurl }}" target="_blank">here</a>. Throughout my PhD I also worked on <a href="{{ '/projects/' }}">multiple other projects</a> related to artificial intelligence and machine learning.
  <br/><br/>
  Before I joined CMU, I graduated with an M.Eng. in <a href="http://www.imperial.ac.uk/electrical-engineering" target="_blank">Electrical and Electronic Engineering</a> from <a href="https://www.imperial.ac.uk/" target="_blank">Imperial College London</a>. For my Master's thesis I proposed a way to use topic modelling methods in order to perform human motion classification.
</div>

<!-- News -->
<div class="news mt-3 p-0">
  <h1 class="title mb-4 p-0">news</h1>
  {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">
        <span class="badge danger-color-dark font-weight-bold text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %-d, %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %}
</div>
