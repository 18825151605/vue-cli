<template>
    <div class="foot">
        <ul>
            <li v-for="(val,i) in list">
                <h3 v-bind:style="{background:color[i]}" @click="dop(i)"></h3>
                <span>{{val}}</span>
            </li>

        </ul>
    </div>
</template>


<script>
export default {
    name: 'foot',
    data() {
        return {
            list: ['首页', '发现', '探索', '发掘'],
            color: ['red', 'yellow', 'blue', 'green']
        }
    },
    methods: {
        dop: function(i) {
            alert(i)
        }
    }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.foot {
    position: fixed;
    bottom: 0;
    width: 100vw;
    height: 60px;
}

.foot ul {
    height: 100%
}

.foot li {
    box-sizing: border-box;
    padding: 10px 30px;
    list-style: none;
    float: left;
    width: 25%;
    height: 100%
}

.foot li h3 {
    height: 20px;
    background: red;
}
</style>