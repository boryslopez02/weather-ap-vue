<template>
  <div class="theme">
    <div class="top-bar">
      <button class="btn-menu">
        <box-icon color="white" name='menu'></box-icon>
      </button>
      <p>{{ day }}</p>
      <span>{{ temperature }}</span>
    </div>

    <div class="mainInfoContainer position-relative">
      <div class="dayInfo">
        <div class="location">
          <h1>Kyiv</h1>
          <div class="indicators">
            <span class="active"></span>
            <span></span>
            <span></span>
            <span></span>
          </div>
        </div>
        <div class="temperature">
          <h1>28°</h1>
          <div class="d-flex">
            <div class="box">
              <box-icon name='chevron-up' color="white"></box-icon>
              <span>31°</span>
            </div>
            <div class="box">
              <box-icon name='chevron-down' color="white"></box-icon>
              <span>19°</span>
            </div>
          </div>
        </div>
        <div class="details">
          <h3>Sunny</h3>
          <p>Feels like 29°</p>
        </div>
      </div>

      <div class="animationDay position-absolute">
        <div class="shadowIcon">
          <box-icon color="white" name='sun' size="300px" class="iconDay"></box-icon>
        </div>
      </div>
    </div>

    <div class="stadistics">
      <div class="dataContainer">
        <div class="timeData">
          <div class="item">
            <span>Ahora</span>
            <h3>28°</h3>
          </div>
          <div class="item">
            <span>1 pm</span>
            <h3>29°</h3>
          </div>
          <div class="item">
            <span>2 pm</span>
            <h3>31°</h3>
          </div>
          <div class="item">
            <span>3 pm</span>
            <h3>31°</h3>
          </div>
          <div class="item">
            <span>4 pm</span>
            <h3>35°</h3>
          </div>
        </div>
      </div>

      <div class="listDays">
        <div class="dayItem">
          <div class="listItem">
            <p>Lunes</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='cloud-rain' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p>100%</p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>

        <div class="dayItem">
          <div class="listItem">
            <p>Martes</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='cloud-rain' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p>50%</p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>

        <div class="dayItem">
          <div class="listItem">
            <p>Miercoles</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='sun' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p></p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>

        <div class="dayItem">
          <div class="listItem">
            <p>Jueves</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='cloud-rain' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p>100%</p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>

        <div class="dayItem">
          <div class="listItem">
            <p>Viernes</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='sun' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p>15%</p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>

        <div class="dayItem">
          <div class="listItem">
            <p>Sabado</p>
          </div>
          <div class="listItem">
            <div class="icon">
              <box-icon name='cloud' color="white" size="25px"></box-icon>
            </div>
            <div class="percentage">
              <p></p>
            </div>
          </div>
          <div class="listItem">
            <div class="changes">
              <p>31</p>
              <span>13</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import moment from 'moment';
moment.lang('es');
export default {
  name: 'App',
  data () {
    return {
      day: moment().format("dddd MMM YYYY"),
      temperature: '°C'
    }
  }
}
</script>

<style lang="sass">
  
</style>
