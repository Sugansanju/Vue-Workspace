<template>
<b-container fluid>
    <b-row style="margin-top: 25px; ">
        <b-col>      
            <student-list :listItems="students"></student-list>
        </b-col>
    </b-row>   
</b-container>    
</template>
<script>
import StudentList from "@/components/comp/misc/StudentList.vue";  
export default {
    name: 'StudentTab',
    components:{
        StudentList,
    },
    data: function(){
        return{
            students:[
                {image: '01.png', name:'Priya Dharshini', contact:'priya@example.com'},
                {image: '02.png', name:'Divya Shri', contact:'9876543210'},
                {image: '03.png', name:'Ram Kumar', contact:'ramkumar@example.com'},
                {image: '04.png', name:'Shri Hari', contact:'srihari@gmail.com'},
                {image: '05.png', name:'Nithya Kalayani', contact:'9876543210'},
                {image: '06.png', name:'Muhamed Farook', contact:'farook@example.com'},
                {image: '07.png', name:'Rishwan', contact:'rishwan@example.com'},
                {image: '08.png', name:'Chinna Raj', contact:'chinnaraj123@example.com'},
                {image: '09.png', name:'Jeya Pandian', contact:'jeyapandian@example.com'},
            ],
        }
    }
};
</script>
