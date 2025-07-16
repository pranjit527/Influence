![Uploading Screenshot_2025-07-15-15-11-34-453_com.google.android.youtube.jpg…]()
# Influenceimport 'package:flutter/material.dart';

void main() {
  runApp(InfluenceApp());
}

class InfluenceApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Influence',
      theme: ThemeData(
        primarySwatch: Colors.deepPurple,
        scaffoldBackgroundColor: Colors.white,
        visualDensity: VisualDensity.adaptivePlatformDensity,
      ),
      home: HomeScreen(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class HomeScreen extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Influence'),
        centerTitle: true,
      ),
      body: Center(
        child: Text(
          'Welcome to Influence!',
          style: TextStyle(fontSize: 24, fontWeight: FontWeight.bold),
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: () {
          // Future feature: Add new post/quote/poll
        },
        child: Icon(Icons.add),
      ),
    );
  }
}
