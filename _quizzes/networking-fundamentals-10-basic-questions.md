---
title: "Networking Fundamentals: 10 Basic Questions"
topic: networking
difficulty: Beginner
duration: 10 mins
description: Here is the quiz with 10 basic networking questions to enhance the
  basic skills.
published: true
questions:
  - question: Which layer of the OSI model is responsible for logical addressing and
      routing packets across different networks?
    options:
      - Network Layer
      - Data Link Layer
      - Transport Layer
      - Physical Layer
    explanation: The Network Layer is the "traffic controller" of the OSI model. It
      uses IP addresses to determine the best path for data to travel across
      different networks. While the Data Link layer handles local hardware
      addresses (MAC), the Network Layer handles global logic.
    correct: Network Layer
  - question: Which networking device connects multiple devices within a LAN and
      forwards data specifically to the destination MAC address?
    options:
      - Hub
      - Router
      - Switch
      - Repeater
    correct: Switch
    explanation: A switch is "smarter" than a hub; it keeps a table of MAC addresses
      to ensure data is sent only to the specific port where the destination
      device is connected.
  - question: If you need to ensure that a file is transferred completely and
      without errors, which protocol should you use?
    options:
      - ICMP
      - UDP
      - IP
      - TCP
    explanation: TCP (Transmission Control Protocol) is connection-oriented and uses
      acknowledgments to guarantee that all data arrives correctly and in order.
    correct: TCP
---
