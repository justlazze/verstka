<template>
<div class="navbar__profile" :class="{'opened': isShow}" @click="toggle">
    <div class="navbar__profile-photo">
        <img src="navbarphoto.svg" alt="">
    </div>
    <div class="navbar__profile-info">
        <div class="navbar__profile-name">
            Oleg K.
        </div>
        <div class="navbar__profile-id">
            ID: 000001
        </div>
    </div>
    <div class="navbar__profile-row">
        <img src="/navbarprofilerow.svg" alt="">
    </div>
    <div class="navbar__profile-menu">
        LOHLOHLOHOHO
    </div>
</div>
</template>

<script>

export default {
    data() {
        return {
            isShow: false,
        }
    },
    methods: {
        toggle() {
            this.isShow = !this.isShow
        },
        show() {
            this.isShow = true
        },
        hide() {
            this.isShow = false
        }
    }
}
</script>

<style lang="scss" scoped>
.navbar__profile {
    width: 213px;
    height: 46px;
    background: #F8F8F8;
    border-radius: 8px;
    display: flex;
    align-items: center;
    padding: 8px;
    cursor: pointer;
    position: relative;
    z-index: 10;
    transition: .2s;
    $root: &;
    &:hover {
        background: #eeeeee;
        transition: .2s;
        #{$root} {
            &-row {
                transition: .2s;
                transform: scale(1.1);
            }
        }
    }
    &.opened {
        height: auto;
        border-radius: 8px 8px 0 0;
        filter: drop-shadow(0px 1px 5.7px rgba(69, 69, 69, 0.2));
        &:hover {
            background: #F8F8F8;
        }
        #{$root} {
            &-menu {
                display: block;
            }
        }
    }
    &-row {
        transition: .2s ease-out;
    }
    &-info {
        margin-left: 12px;
        flex: auto;
    }
    &-id {
        font-size: 12px;
        font-weight: 400;
        color: #7F8086;
    }
    &-name {
        font-size: 14px;
        color: #404040;
        font-weight: 600;
    }
    &-photo {
        img {
            display: block;
        }
    }
    &-menu {
        position: absolute;
        top: 100%;
        right: 0;
        background: #fff;
        border-radius: 0 0 8px 8px;
        z-index: 10;
        display: none;
        height: 200px;
        width: 100%;
    }
}
</style>