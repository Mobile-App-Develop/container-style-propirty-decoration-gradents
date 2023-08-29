# container-style-propirty-decoration-gradents
import 'package:flutter/material.dart';

void main() {
  runApp(
    MyStatelessWidget(),
  );
}

class MyStatelessWidget extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text("Container Widget"),
        ),
        body: Material(
          child: Container(
            width: 200,
            height: 150,
            //color: Colors.yellow,
            alignment: Alignment.topRight,
            
            child: Text("KHADIM",
              //textDirection: TextDecoration.rtl,
              textAlign: TextAlign.justify,
                            overflow: TextOverflow.ellipsis, // zayda text honi ki sarorat  me ..... lga dy ga
              softWrap: false, // ak line jo jeta text a sky bs  wohi dekhay
              maxLines: 2, // jetni line ka text dekhan ho
              //child: Text("#",
           // semanticsLabel: "my code", //user ky ly text me # nazar ay ga lekin is me hum apni yadast ky ly jo marzi likh lain
STYLE PROPORITY
 style: TextStyle ( fontFamily: "TiltPrism", color: Colors.white,
              //textScaleFactor:5, // text ka size zayda krna
              fontStyle: FontStyle.italic,
                fontWeight: FontWeight.bold,
                fontSize: 30,
                letterSpacing: 13,
                wordSpacing: 12,
                height: 1

                                 //backgroundColor: Colors.grey,
              ),
              ),



            margin: EdgeInsets.only(left: 100, right: 50, bottom: 40, top: 200),
            //padding: EdgeInsets.only(left: 10, right: 20, bottom: 30, top: 40),
            decoration: BoxDecoration(
              color: Colors.blue,
              shape: BoxShape.rectangle,
              border: Border.all(width: 3, color: Colors.black),
             borderRadius: BorderRadius.only( // APNI MARZI CORNER BANANA
               topLeft: Radius.elliptical(420, 420),
               topRight: Radius.elliptical(420, 420),
               bottomLeft: Radius.elliptical(420, 420),
               bottomRight: Radius.elliptical(420, 420),
             ),
             // borderRadius: BorderRadius.circular(335),
              //borderRadius: BorderRadius.only(
               // bottomRight: Radius.elliptical(50, 50),
                //bottomLeft: Radius.elliptical(50, 50),
                //topRight: Radius.elliptical(50, 50),
                //topLeft: Radius.elliptical(50, 50),
              //),
              gradient: LinearGradient(
                begin: Alignment.centerLeft,
                end: Alignment.topLeft,
                colors: [Colors.orange, Colors.red,Colors.yellow],
              ),
              ),
            ),
          ),
          /*child: Container(
            width: 300,
            height: 250,
            child: Text(
              "Hello World",
              style: TextStyle(fontSize: 25),
            ),

            margin: EdgeInsets.only(left: 50, top: 50),
            padding: EdgeInsets.all(30),

            decoration: BoxDecoration(
              color: Colors.orange,
              shape: BoxShape.rectangle,
              gradient: LinearGradient(
                begin: Alignment.topRight,
                end: Alignment.bottomLeft,
                stops: [0.2, 0.5, 0.8, 0.9],
                colors: [
                  Colors.brown,
                  Colors.white,
                  Colors.green,
                  Colors.yellow
                ],
              ),
              borderRadius: BorderRadius.only(
                bottomRight: Radius.elliptical(50, 50),
                bottomLeft: Radius.elliptical(50, 50),
                topRight: Radius.elliptical(50, 50),
                topLeft: Radius.elliptical(50, 50),
              ),
              border: Border.all(width: 10, color: Colors.pink),
            ),
          ),*/
        ),

    );
  }
}
