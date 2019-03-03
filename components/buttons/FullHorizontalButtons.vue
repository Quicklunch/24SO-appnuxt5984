<template>
  <div class="col-md-12 hrfull-btnalign" style="text-align: center;">
    <div class="table">
      <hr>
      <span class="hrfull-buttons">
        <div class="container">
          <div class="row">
            <div class="col-md-5">
              <div class="btn-group" id="status" data-toggle="buttons">
                <label class="btn btn-default btn-on btn-lg active">
                  <input type="radio" value="1" checked="checked">
                  <span>Pakker</span>
                </label>
                <label class="btn btn-default btn-off btn-lg">
                  <input type="radio" value="0">
                  <span style="color:#2299FF;">Enkeltmoduler</span>
                  <span>fra 99,-</span>
                </label>
              </div>
            </div>
          </div>
        </div>
      </span>
    </div>
  </div>
</template>

<style>
.hrfull-btnalign {
  text-align: center;
  float: left;
  width: 100%;
  height: 5rem;
  margin-top: 6rem;
}

hr {
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
}
.hrfull-buttons {
  display: inline-block;
  position: relative;
  top: -3rem;
  text-align: center;
  width: 500px;
}

.btn-default {
  min-width: 250px;
}

.table {
  display: table;
  width: 100%;
  height: 100%;
  position: absolute;
}

.table-cell {
  display: table-cell;
  text-align: center;
  vertical-align: middle;
  width: auto;
  height: auto;
  z-index: 100;
}
.hrfull-btnbox {
  height: auto;
  margin: 2rem auto;
  width: 516px;
  display: flex;
}
.hrfull-button {
  margin: 2rem auto;
}

.hrfull-btnbox .btn-lg {
  width: 50%;
}

.btn-group {
  width: 516px;
  height: 52px;
}

.btn-default.btn-on.active span {
  color: #fff;
}

.btn-default.btn-on.active {
  background-color: #2299ff;
  color: white;
  border: 1px solid #2299ff;
}

.btn-default.btn-off.active {
  background-color: #2299ff;
  color: white;
  border: 1px solid #2299ff;
}

@media screen and (max-width: 990px) {
  .btn-default {
    min-width: 100%;
    margin: 1rem;
    border-radius: 0px;
  }
  .hrfull-buttons {
    width: 100%;
  }
  .hrfull-btnalign {
    height: 16rem;
  }
  .btn-group {
    width: 100%;
    height: 52px;
  }
}
</style>