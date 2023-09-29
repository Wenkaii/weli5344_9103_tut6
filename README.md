# weli5344_9103_tut6


The "Matrix Effect," famously known as "Bullet Time," is a visual effect that depicts action sequences in slow motion while the camera appears to move around the scene at normal speed. This technique became iconic through its use in "The Matrix" film series and has inspired countless recreations and adaptations in other movies, video games, and various media.

Part 1: 
Imaging Technique Inspiration
Technique: Bullet Time
I am inspired by the Bullet Time technique for its ability to provide a detailed, multifaceted view of intense, fleeting moments, allowing the audience to observe details that would be impossible to catch in real time. This approach can offer a unique, immersive perspective on visual storytelling, enabling a deeper exploration and understanding of depicted events and scenes.

images
![1-16](https://github.com/Wenkaii/weli5344_9103_tut6/assets/146446712/c8cee10a-38f3-4371-900a-119889fded9b)
![1652d6630580f407~tplv-t2oaga2asx-jj-mark_3024_0_0_0_q75](https://github.com/Wenkaii/weli5344_9103_tut6/assets/146446712/092dac2b-5e38-4b97-b9a3-dabcd08befc3)



Part 2

The code
https://dev.to/gnsp/making-the-matrix-effect-in-javascript-din


In each frame, we need to render a semi transparent black rectangle on top of the previous frame, so that the characters rendered in previous frames can look progressively dimmed. Then we need to render the new characters at the end of each column for the current frame.

They coordinates for each column is stored in the ypos array. In each frame we want to randomly reset some columns to start from the top again, so that it seems like columns of varying heights are falling from the top. For the rest of the columns we will simply move the y coordinate 20px down, so that in next frame a new character appears below the current one.

