import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  final List<String> items = [
    'Groceries',
    'Workout',
    'Read a Book',
    'Call Mom',
    'Write Code',
    'Take a Walk',
    'Cook Dinner',
    'Watch a Movie',
    'Water Plants',
    'Plan Vacation',
    'Learn Flutter',
    'Play Guitar',
    'Meet Friends',
    'Go for a Run',
    'Clean House',
    'Practice Meditation',
    'Visit Library',
    'Listen to Music',
    'Shop for Clothes',
    'Write Journal',
  ];

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Simple ListView Example'),
        ),
        body: ListView.builder(
          itemCount: items.length,
          itemBuilder: (context, index) {
            return ListTile(
              title: Text(items[index]),
              onTap: () {
              },
            );
          },
        ),
      ),
    );
  }
}
