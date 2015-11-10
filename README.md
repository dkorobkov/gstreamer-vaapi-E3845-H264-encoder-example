# gstreamer-vaapi-E3845-H264-encoder-example
Modification of test-appsrc from gst-rtsp-server that works with Intel Atom E3845 CPU hardware H.264 encoder through vaapiencode_h264. 

It took a while to find and adjust these tricky parameters to enable vaapiencode_h264!

The aim was to stream RTSP into video management systems. 

This modified example occupies 75-80% of 400% (4-core) 1.9 GHz E3845 CPU 
encoding FullHD video at 30 FPS. 

A fix (probably ugly but working) is added to remove memory leak in 
test_appsrc on long runs.
