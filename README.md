


import 'dart:html';

import 'package:flutter/material.dart';
import 'package:flutter/src/foundation/key.dart';
import 'package:flutter/src/widgets/framework.dart';

class homepage extends StatefulWidget {
   homepage({Key? key}) : super(key: key);

  @override
  State<homepage> createState() => _homepageState();
}

class _homepageState extends State<homepage> {
       String number= "?";
       String number2= "?";
     Color appCo = Colors.pink;
  @override
  Widget build(BuildContext context) {
    
           return Scaffold(
              backgroundColor: Color.fromARGB(255, 174, 156, 162),
              appBar: AppBar(
                backgroundColor: Color.fromARGB(255, 96, 74, 81),
                centerTitle: true,
                title: Text(" page 1"),
                leading: Icon(Icons.menu),
                actions: [
                  Icon(Icons.person),
                  Center(
                   child: Text("hello waad"),

                  ),
                  SizedBox(
                    width: 20,

                  ),
                ],
              ),


                 body: ListView( children: [
                          Center( child :
                       Text("what is result for the operation? "),
                       ),
              
                  Center(

                 child :
                 Text(" 2 +2 = ${number}"),
                       
                  ),
                  TextButton(
                    onPressed: () {
                   print("befor add "+number);    
                    setState(() {   
                       number= "4";
                      
                    });
                    print("After add "+number);
                    },
                  
                     child: Icon(Icons.add),
                
                     ),

                   Center(

                    child: Text("2 + 3 = ${number2}"),

                   ),
                    TextButton(onPressed: () {

                      setState(() {
                        number2= "5";
                      });
                    },
                    
                    
                     child: Icon(Icons.add)),
                 ],
                 
                 ),

           );
  }
}

  List carInfo=[
   {
     "color" :"2+3",
    "model" : 2022,
    "price" : 874895,
    "descrip" :" fast ",
    "image": "images/images1.jpg",
    
   },
     
       {
     "color" :"white",
    "model" : 2018,
    "price" : 585030,
    "descrip" :" fast ",
    "image": "images/images1.jpg",
   },

      {
     "color" :"blue",
    "model" : 2017,
    "price" : 2484939,
    "descrip" :" fast ",
    "image": "images/images1.jpg",
   },

  ];

 
