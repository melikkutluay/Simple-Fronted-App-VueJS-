<template>
    <div class="component">
        <h1>The User Component</h1>
        <p>I'm an awesome User!</p>
        <hr>
        <div class="row">
            <div class="col-xs-12 col-sm-6">
                <app-user-detail
                :myName="name"
                @nameWasReset="name = $event"
                :userAge="age"></app-user-detail>
            </div>
            <div class="col-xs-12 col-sm-6">
                <app-user-edit :userAge="age"></app-user-edit>
            </div>
        </div>
    </div>
</template>

<script>
    import UserDetail from './UserDetail.vue';
    import UserEdit from './UserEdit.vue';

    export default {
        data:function(){
          return{
              name : 'Melik',
              age : 27
          }
        },
        components: {
            appUserDetail: UserDetail,
            appUserEdit: UserEdit
        }
    }
</script>

<style scoped>
    div {
        background-color: lightblue;
    }
</style>
