---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<style>
.banner{
    content: url("/assets/img/gen-small.jpg");
    width:40%; 
    margin:0px;
    margin-top:13px;
    margin-left:10px;
    clear:right;
    float:right;
}
.video{
    margin:0;
    margin-bottom: 0px;
    margin-left: 10px;
    width:40%; 
    clear:right;
    float:right;
}
.ads{
    width:40%; 
    margin:10px;
    margin-top:20px;
    margin-left:10px;
    clear:right;
    float:right;
    }
.sum{
    color:#838996;
    background-color:#f5f5f5;
    /*background-color:lightblue; */
    padding:20px;
    /*margin:0px; */
    }
a{
    color:black;
}

@media (max-width: 600px) {
    .banner{
        float: none;
        display: block;
        margin-left: auto;
        margin-right: auto;
        margin-top:0;
        content: url("/assets/img/banner-small.png");
        width: 100%
    }
    .video{
        display:none;
    }
    .ads{
        float: none;
        width: 90%;
    }
}
</style>

<h1 style="margin-bottom:0px">Autonomous Vehicle Lab </h1>
<img class='banner'/>
<iframe src="https://youtube.com/embed/k4qmW9vgAio" class='video' frameborder="0"> </iframe>
<a href="tutorials"><img class="ads" src="/assets/img/sys-summer-2022.jpg"/></a>
<p class="sum">
Welcome to the Autonomous Vehicle Lab (AV-Lab) at <a href="https://ku.ac.ae">Khalifa University</a>! Our research focuses on Autonomous Vehicle (AV) technologies and the integration aspects into smart cities.
<b>Safety assurance</b> is a significant barrier to deploying AVs on a massive scale due to technical challenges that arise from the uncertain environment, such as road and weather conditions, behavioral uncertainty of pedestrians and surrounding vehicles, and modeling inaccuracies. </p>
Our research revolves around the following questions:
- How can we build safety within and around the core components of AV decision-making pipeline?
- How can each component reasonably report and parse uncertainty from dependent ones in an efficient and explainable manner?
- How can we build decision-making schemes that take the best out of the machine learning community and the rigor of theoretical computer science to achieve provably safer schemes without sacrificing efficiency?
- What are the ways to exploit enabler technologies such as vehicle-to-everything (V2X) to build multi-agent solutions to realistic problems?
