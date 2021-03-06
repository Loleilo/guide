# Guide

Soon this will contain info on how the API works, how to make a widget, etc.

## Roadmap

 1. Implement basic structure of backend, sensor firmware, and frontend - **v1.0.0**
      - Backend:
        - Simple access/no access permission system
        - Build atom/group/user model
        - Store user preferences/dashboard
      - Sensor:
        - User configurable
        - Remembers user's settings
        - User can configure through wifi network
        - Auto creation of needed entities
      - Frontend:
        - Displays atoms and group users own
        - Allows user to see atom values and edit
        - User configurable dashboard
            - User can choose and customize widgets to display on dashboard
      - Proper versioning system
            
 2. NodeJS rewrite - **v2.0.0**
      - Use MongoDB and NodeJS
      - Replace object polling system with WebSockets event based system

 3. Proper permission system
      - Based on 3 tiers: Owner, Can edit, Can view **v2.0.1**
        - Tiers inherit permissions from below levels, Edit permssions also gives View permssions. Owner has all 3 permissions
      - Role system for users: Admin and user **v2.0.2**
        - Should be extensible to more roles
 
 2. Security fixes - **v2.0.3**
      - Escaping: JSON, MySQL, HTML/React (shouldn't need escaping, but be careful)
      - SQL injection test with sqlmap
      - Remote all testing code
