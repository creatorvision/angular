// IT contains extra code blocks developed to learn things in angular.


  //     // // Making a Provider to return a text value 
    //     // demoApp.provider("myProvider", function() {
    //     //     this.$get = function() {
    //     //         return "My Value";
    //     //     };
    //     // });  

    //     // Making an object to be called from the factory to return its value 
    //     function myObject(){
    //         this.getValue = function(){
    //             return "My value from the object";
    //         };
    //     }
    //     // Making a factory to return a text value
    //     demoApp.factory("myProvider",function(){
    //         console.log("factory function is called");
    //         //return "My Value"; // return normal text value
    //         return new myObject(); // Returning the whole object to the controller.
    //     });

    //     // // Factory with inbuild function object
    //     // demoApp.factory("myProvider", function() {
    //     //     console.log("Factory function called.");
    //     //     return new function() { // INLINED our object constructor
    //     //         this.getValue = function() {
    //     //             return "My Value";
    //     //         };
    //     //     };
    //     // });

    //     demoApp.controller('MyController',function(myProvider){
    //         //console.log("MyController - myProvider: " + myProvider);
    //         console.log("MyController - myProvider: " + myProvider.getValue());
    //     }); 
    //     demoApp.controller('MyController2',function(myProvider){
    //         //console.log("MyController2 - myProvider:"+ myProvider); // Provider only "get" once , no matter how many times provider is injected.
    //         console.log("MyController2 - myProvider:"+ myProvider.getValue());
    //    });