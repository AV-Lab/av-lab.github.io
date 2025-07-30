---
layout: page
title: About
show_menu: true
---
<img src="/assets/img/eyad-av.jpg" width=300 class="img-right" />
<p class="justified-text">
AV-lab is part of <a href="https://www.ku.ac.ae/kucars">KU Center for Autonomous Robotic Systems (KUCARS)</a> focused on advancing autonomous and robotic technologies through four main themes and nine integrated projects over three years. The themes include Autonomous Cars, Aerial Robotics, Marine Robotics, and Industrial Robotics.
</p>

<p class="justified-text">
<a href="https://docs.google.com/forms/d/e/1FAIpQLSeMoTvLyh_yrqTJCfM6vkH0RTbbu2YDuFw5VTYXGfFaDKLmig/viewform"> <img width=100 class="icon" src="/assets/img/apply-icon.jpg"/> </a>
If you are interested in working with us, please submit your application through our online <a href="https://docs.google.com/forms/d/e/1FAIpQLSeMoTvLyh_yrqTJCfM6vkH0RTbbu2YDuFw5VTYXGfFaDKLmig/viewform">form</a>.
For any collaboration or technical inquires, please contact Eng. Mohammed Riyadh:
Email: mhdriadh.alkharrat@ku.ac.ae.
</p>

# Our Labs
<div class="labs-container">
  <div class="lab-section">
    <div class="lab-title">Main Campus Lab</div>
    <p>Lab B2-0033, Building B</p>
    <div class="map-container">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d232454.3459404653!2d54.131226539611795!3d24.447344928081886!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3e5e686120c31b23%3A0x5d25df2e9ffa142e!2sKhalifa%20University!5e0!3m2!1sen!2sae!4v1658386324220!5m2!1sen!2sae" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" class="map-iframe"></iframe>
    </div>
  </div>
  
  <div class="lab-section">
    <div class="lab-title">SAN Campus Test Facility</div>
    <p>Wind Tunnel Building</p>
    <div class="map-container">
      <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d29062.311991762977!2d54.48664131685789!3d24.423396898780354!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3e5e43e774701f6b%3A0xd6c04bcea62eb533!2zMjTCsDI1JzA4LjUiTiA1NMKwMzAnMDMuOCJF!5e0!3m2!1sen!2sae!4v1658386693355!5m2!1sen!2sae" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" class="map-iframe"></iframe>
    </div>
  </div>
</div>


<style>
.icon{
    margin: 5px;
    width: 50px;
    float: left;
}
@media (max-width: 600px) {
    .img-right{
        float: none;
        display: block;
        margin-left: auto;
        margin-right: auto;
    }
}
@media (min-width: 600px) {
    .img-right{
        float: right;
        clear: right;
        width: 300px;
        margin-bottom: 10px;
        margin-left: 15px;
    }
    .logo{
        width: 150px;
    }
}

.justified-text {
    text-align: justify;
}

.labs-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
}

.lab-section {
    flex: 1;
    min-width: 300px;
    display: flex;
    flex-direction: column;
}

.lab-title {
    font-weight: bold;
    font-size: 1.2em;
    margin-bottom: 10px;
}

.map-container {
    flex-grow: 1;
    position: relative;
    width: 100%;
    height: 350px !important;
}

.map-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

@media (max-width: 768px) {
    .labs-container {
        flex-direction: column;
    }
    
    .lab-section {
        width: 100%;
    }
    
    .map-container {
        height: 300px !important;
    }
}
</style>
