<template>
  <div class="container">
      <div class="card">
          <div>
              <img class="card-img" src='https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortWaved&accessoriesType=Prescription01&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=Blue03&eyeType=Default&eyebrowType=Default&mouthType=Twinkle&skinColor=Light'/>
          </div>
          <div class="card-text">
              <h2 class="card-title">Gaurav Gawade</h2>
              <p class="card-description">
                 <span>Lorem ipsum dolor sit amet consectetur, adipisicing eli.</span> 
              </p>
              <ul class="card-skills">
                  <li class="skill">UI Designer.</li>
                  <li class="skill">UX Designer.</li>
                  <li class="skill">Web Developer.</li>
              </ul>
              <a href="#" class="card-link">Read More</a>
          </div>
      </div>
      <div class="skeleton">
          <div class="skeleton-img"></div>
          <div class="skeleton-text">
              <h2 class="skeleton-title"></h2>
              <p class="skeleton-description">
                <span></span>
                <span></span>
              </p>
              <ul class="skeleton-skills">
                  <li class="skill"></li>
                  <li class="skill"></li>
                  <li class="skill"></li>
              </ul>
              <a href="#" class="skeleton-link"></a>
          </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    li{
        list-style: none;
    }

    .card,
    .skeleton {
      display: flex;
      justify-content: space-around;
      padding: 20px;
      max-width: 400px;
      height: 155px;
      margin: 20px;
      border-radius: 10px;
      background-color: #E2E8F0;
      box-shadow:
        0 9px 33px rgba(0, 0, 0, 0.07);
    }

    .card-text, .skeleton-text{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        width: 250px;
        margin-left: 10px;
    }

    .card-img, .skeleton-img{
        width: 75px;
        height: 75px;
        border-radius: 50%;
    }

    
    .card-description, .skeleton-description{
        margin: 10px 0;
    }

    .card-link, .skeleton-link{
        margin-top: 20px;
    }

    .card-skills , .skeleton-skills{
        display: flex;
        justify-content: space-between;
    }

    .card-img{
        background-color: #4F46E5;
    }

    .card-title{
        font-size: 16px;
        color: #334155;
    }

    .card-description{
        font-size: 12px;
        color: #64748B;
    }

    .card-skills .skill {
        font-size: 12px;
        font-weight: 600;
        color: #475569;
    }

    .card-link{
        font-size: 12px;
        color: #4F46E5;
    }

    .skeleton-title{
        width: 150px;
        height: 12px;
        /* background-color: #94A3B8; */
        animation: pulse 2s infinite ease-in-out;
    }

    .skeleton-img{
        animation: pulse 2s infinite ease-in-out;
    }

    .skeleton-description span:nth-child(1){
        display: block;
        width: 210px;
        height: 10px;
        /* background-color: #94A3B8; */
        animation: pulse 2s infinite ease-in-out;
    }

    .skeleton-description span:nth-child(2){
        display: block;
        width: 150px;
        height: 10px;
        /* background-color: #94A3B8; */
        animation: pulse 2s infinite ease-in-out;
        margin-top: 5px;
    }

    .skeleton-skills .skill{
        width: 65px;
        height: 12px;
        /* background-color: #94A3B8; */
        animation: pulse 2s infinite ease-in-out;
    }

    .skeleton-link{
        width: 75px;
        height: 12px;
        /* background-color: #94A3B8; */
        animation: pulse 2s infinite ease-in-out;
    }

    @keyframes pulse {
        0% {
            background-color: #94A3B8;
        }

        50% {
            background-color: #CBD5E1;
        }

        100% {
            background-color: #94A3B8;
        }
    }

    .container{
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
  }
</style>