# threejs-shadertoy
An experimental project trying to run [shadertoy](https://www.shadertoy.com/) shaders using threejs.

### Supported Shadertoy uniforms
- [ ] uniform vec3      iResolution;           // viewport resolution (in pixels)
- [ ] uniform float     iTime;                 // shader playback time (in seconds)
- [ ] uniform float     iTimeDelta;            // render time (in seconds)
- [ ] uniform float     iFrameRate;            // shader frame rate
- [ ] uniform int       iFrame;                // shader playback frame
- [ ] uniform float     iChannelTime[4];       // channel playback time (in seconds)
- [ ] uniform vec3      iChannelResolution[4]; // channel resolution (in pixels)
- [ ] uniform vec4      iMouse;                // mouse pixel coords. xy: current (if MLB down), zw: click
- [ ] uniform samplerXX iChannel0..3;          // input channel. XX = 2D/Cube
- [ ] uniform vec4      iDate;                 // (year, month, day, time in seconds)
- [ ] uniform float     iSampleRate;           // sound sample rate (i.e., 44100)

### More features
 - Scaling: Adjust fragment shader resolution. Can be reduced to improve performance for shaders with less finer details. 
 - Post processing: Built in brightness, saturation and other effects.
 - FPS control: Adjust frame-rate. Can be reduced to improve performance for shaders with slow/subtle movement.
 - Playback control: Start/Pause playback.
- dat.GUI util: Generate dat.gui for shader uniforms.