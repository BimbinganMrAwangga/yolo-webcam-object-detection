# YOLO Webcam Object detection

[![HitCount](http://hits.dwyl.io/AlbertSuarez/yolo-webcam-object-detection.svg)](http://hits.dwyl.io/AlbertSuarez/yolo-webcam-object-detection)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/AlbertSuarez/yolo-webcam-object-detection)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![GitHub stars](https://img.shields.io/github/stars/AlbertSuarez/yolo-webcam-object-detection.svg)](https://GitHub.com/AlbertSuarez/yolo-webcam-object-detection/stargazers/)
[![GitHub forks](https://img.shields.io/github/forks/AlbertSuarez/yolo-webcam-object-detection.svg)](https://GitHub.com/AlbertSuarez/yolo-webcam-object-detection/network/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/AlbertSuarez/yolo-webcam-object-detection.svg)](https://github.com/AlbertSuarez/yolo-webcam-object-detection)

🎥 Real-time object detection from a Webcam using tiny-YOLO or YOLO with [Darkflow](https://github.com/thtrieu/darkflow) (Darknet + tensorflow).

## Contents

1. [Requirements](#requirements)
2. [Recommendations](#recommendations)
3. [Usage](#usage)
4. [Example](#example)
5. [Authors](#authors)
6. [License](#license)

## Requirements

- Python 3+.

## Recommendations

Usage of [virtualenv](https://realpython.com/blog/python/python-virtual-environments-a-primer/) is recommended for package library / runtime isolation.

## Usage

To run the application, please execute the following from the root directory:

1. Setup virtual environment.

2. Install dependencies.

  ```bash
  pip3 install -r requirements.lock
  ```

3. Install [Darkflow](https://towardsdatascience.com/yolov2-object-detection-using-darkflow-83db6aa5cf5f)

  ```bash
  source install_darkflow.sh
  ```

4. Run the application with one of the available models (`tiny-yolo-voc` or `yolo`)

  ```bash
  python3 -m src [--model MODEL_NAME --device_id DEVICE_ID]
  ```

  > `tiny-yolo-voc` is the default model in order to get a better performance w/o GPU. If you want to get better results, then specify the `yolo` model.
  > `0` is the default device id which is the embedded web cam of your computer. For running the project with another web cam, just specify 1, 2, etc (depends on how many web cams you have).

## Example

![Example](docs/example.png)

## Authors

- [Albert Suàrez](https://github.com/AlbertSuarez)

## License

MIT © YOLO Webcam Object detection
