<template>
    <div class="search">
        <input id='test' type="text"  @focus="del($event)" @blur="reset($event)" value="搜索">
        <!-- <span>{{alert}}</span>
            <span v-for="val in mode">{{ val }}</span> -->
    </div>
</template>
<script>
export default {
    name: 'search',
    data() {
        return {
            message: 'Hello world!',
            alert: '搜索',
            mode: ['123', '345', '456']
        }
    },
    methods: {
        del: function(self) {
           console.log(self.target.value);
            if (self.target.value == this.alert) {
               
                self.target.value = ''
            }
        },
        reset:function (self) {
            console.log(self.target.value);
               if (self.target.value == '') {
                self.target.value = this.alert
            }
        }
    }
}
</script>

   


<style scoped>
.search {
    width: 100vw;
    height: 30px;
    background-color: red;
    display: table-cell;
    vertical-align: middle;
}

input {
    outline: none;
    border: none;
    width: 90%;
    text-align: center;
    height: 20px;
    -webkit-border-radius: 3px;
    -moz-border-radius: 3px;
    -ms-border-radius: 3px;
    -o-border-radius: 3px;
    border-radius: 3px;
}
</style>
