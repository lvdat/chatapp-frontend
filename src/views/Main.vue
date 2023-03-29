<template>
    <div class="container-xxl messhive--main">
        <div class="row messhive--main__row">
            <div class="col-md-4 messhive--main__menu">
                <div class="row text-center messhive--main__menu--toolbar">
                    <div class="col-2 messhive--main__menu--toolbar__dropdown">
                        <div class="dropdown">
                            <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                                <i class="far fa-circle-user"></i>
                            </button>
                            <ul class="dropdown-menu">
                                <li><a class="dropdown-item" href="#">Action</a></li>
                                <li><a class="dropdown-item" href="#">Another action</a></li>
                                <li><a class="dropdown-item" href="#">Something else here</a></li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-10 messhive--main__menu--toolbar__search">
                        <div class="input-group">
                            <input type="text" class="form-control messhive--main__menu--toolbar__search--input" placeholder="Tìm kiếm..." aria-label="Username" aria-describedby="basic-addon1">
                        </div>
                    </div>
                </div>

            </div>
            <div class="col-md-8 messhive--main__message">

            </div>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style>
.messhive--main__row {
    height: 100vh;
    border: 1px solid #ced4da;
}
.messhive--main__row {

}
.messhive--main__menu {
    border-right: 1px solid #ced4da;
}
.messhive--main__message {

}
.messhive--main__menu--toolbar {
    margin-top: 10px;
    padding: 0 15px 10px 10px;
    border-bottom: 1px solid #ced4da;
    max-height: 60px;
}
.messhive--main__menu--toolbar__search--input {
    border-radius: 0%;
}

.dropdown-menu {
  transition: all 0.1s ease;
  transform: scale(0);
  transform-origin: top center;
  padding: 9px;
}
.show .dropdown-menu {
  transform: scale(1);
}
li~.dropdown-item:hover {
    border-radius: 20%;
}
button.dropdown-toggle {
    border-radius: 0%;
    background-color: #fff;
    color: #000;
    border: none;
}
button.dropdown-toggle:hover {
    background-color: unset;
    color: #000;
}
</style>