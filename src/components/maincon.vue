<template>
    <div class="maincon">
        <div class="list" v-for="val in list">
            <div class="left">
                <span>{{val.left}}</span>
            </div>
            <div class="right">
                <span>{{val.right}}</span>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'maincon',
    data() {
        return {
            list: [
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
                { left: '123123', right: '1235345' },
            ]
        }
    },
    methods: {

    }
}
</script>
   


<style scoped>
.maincon {
    width: 100vw;
    height: 80px;
    display: table;
}

.maincon .list>div {
    float: left;
    height: 80px;
    display: table-cell;
    vertical-align: middle;
    line-height: 80px;
    text-align: center;
}

.maincon .list>div span {
    display: inline-block;
}

.maincon .left {
    width: 20%;
}

.maincon .right {
    width: 80%;
}
</style>
