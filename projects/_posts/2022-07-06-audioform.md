---
layout: post
author: Brady Boettcher
---
![theme logo](/images/audioform.png)

Audioform is an audio visualizer for Windows built with Unity3D. It only works for Windows because it's able to grab the system sound output directly, avoiding any routing to start visualization right away. This feature is a bit more difficult for other platforms, but probably possible (any interested developers are welcome to contribute!).

The visualization works by extracting the frequency spectrum amplitudes for each frame and constructing a connected mesh that forms the appearance of a continuous tube. The amplitudes determine the color and radius of the point on the mesh, making it jump around to follow the music.

This project hasn't been touched in a few years, but is still functional and lots of fun! You can grab the code for the project [here](https://github.com/bboettcher3/Audioform).

Click the below images to watch Audioform in action:
[![](https://img.youtube.com/vi/kDEvmMUrX-U/0.jpg)](https://www.youtube.com/watch?v=kDEvmMUrX-U)

[![](https://img.youtube.com/vi/QFyjRExzXVY/0.jpg)](https://www.youtube.com/watch?v=QFyjRExzXVY)