# Boids!

This application is the result of the second assignment turned in under University of New England's COSC250 unit, in 2019. The application is implemented in Scala and is based off Craig Reynold's artificial life program from 1986 (**https://en.wikipedia.org/wiki/Boids**). 
A skeleton code was provided but the majority of this work is my own.

Each boid has a position and velocity, and each boid's next position is calculated according to 'newPosition = position + velocity' where 'newVelocity = velocity + acceleration'. Acceleration for each boid is based on 3 forces that act on it: Separation, Alignment and Cohesion.
Boids will try to move away from other boids if they are too close, will attempt to match the direction and velcity of other boids within 50 pixels, and will attempt to steer towards the middle of other boids within 50 pixels. 
Velocity and acceleration are capped.
Some properties have been added, namely: wind factor, the ability to apply a ramdom vector to each boid in the next frame as if they've been 'startled', and the ability to add boids.

This application demonstrates my ability to write functional code (though some of it is unavoidably imperative, for eg the action replay memory) along with my overall coding style. 

This program is written in Scala and utilises the SBT, any IDE that supports these two will run the program just fine. 
