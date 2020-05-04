# issue-gridsome-bs-collapse

This repo represent the issue I am getting while using gridsome for my documentation.

## Issue

When I import component from outside of gridsome folder it throws error when I collapse the component.
  
However, when I import same component from gridsome package folder it works fine.

## How to run this project

* Intall dependecies in both projects (root & docs)
* run server of both projects
* Toggle through button in vue code
* open docs server(gridsome) and visit /docs path and toggle using button (You will get error in console)
* Try to import collapse component in gridsome(check main.js) from component folder and toggle (It works!! Why??)
