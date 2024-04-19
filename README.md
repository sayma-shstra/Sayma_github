# Sayma_github
This is my first Git Repository.
Dart Programming Code:
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: MyHomePage(),
    );
  }
}

class MyHomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Icons and Text'),
      ),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            // First Icon: Eclipse with Purple Color and Text
            _buildIconWithText(
              icon: Icon(
                Icons.circle,
                size: 100,
                color: Colors.purple,
              ),
              text: 'Sayma Firoj Momin\nPeth Vadgaon',
            ),
            SizedBox(height: 20), // Spacer between icons
            // Second Icon: Add your desired icon and text here
            _buildIconWithText(
              icon: Icon(
                Icons.computer_sharp,
                size: 50,
                color: Colors.blue,
              ),
              text: 'Kolhapur Institute of Technology, Kolhapur',
            ),
            SizedBox(height: 20), // Spacer between icons
            // Third Icon: Add your desired icon and text here
            _buildIconWithText(
              icon: Icon(
                Icons.folder_copy_rounded,
                size: 60,
                color: Colors.black26,
              ),
              text: 'Any Projects',
            ),
            SizedBox(height: 20), // Spacer between icons
            // Fourth Icon: Add your desired icon and text here
            _buildIconWithText(
              icon: Icon(
                Icons.email,
                size: 40,
                color: Colors.brown,
              ),
              text: 'miss.sayma04@gmail.com',
            ),
            SizedBox(height: 20), // Spacer between icons
            // Fifth Icon: Add your desired icon and text here
            _buildIconWithText(
              icon: Icon(
                Icons.phone_in_talk,
                size: 30,
                color: Colors.green,
              ),
              text: 'Mobile Number',
            ),
          ],
        ),
      ),
    );
  }

  Widget _buildIconWithText({required Icon icon, required String text}) {
    return Row(
      children: [
        Padding(
          padding: const EdgeInsets.symmetric(horizontal: 20),
          child: icon,
        ),
        SizedBox(width: 10), // Spacer between icon and text
        Expanded(
          child: Text(
            text,
            style: TextStyle(fontSize: 20),
          ),
        ),
      ],
    );
  }
}
