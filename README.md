# People Counting OpenCV on RasPi 3B

## Run people counting with Movidius NCS(one) on RasPi 3B
python people_counter.py \
--prototxt mobilenet_ssd/MobileNetSSD_deploy.prototxt \
--model mobilenet_ssd/MobileNetSSD_deploy.caffemodel \
--input videos/example_01.mp4 \
-g mobilenetgraph_frdc25403

## Run people counting without Movidius NCS(one) on RasPi 3B
python people_counter_old.py \
--prototxt mobilenet_ssd/MobileNetSSD_deploy.prototxt \
--model mobilenet_ssd/MobileNetSSD_deploy.caffemodel \
--input videos/example_01.mp4
