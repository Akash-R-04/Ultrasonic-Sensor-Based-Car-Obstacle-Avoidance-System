# 🤖 Obstacle Avoidance Robot Car using Arduino

This project is an Arduino-based four-wheel robot car that uses an ultrasonic sensor mounted on a servo motor to detect and avoid obstacles. The car can move forward, backward, turn left, turn right, and stop, based on the obstacle detection logic.

## 📜 Description

- **Motors**: Controlled using the Adafruit Motor Shield library (`AFMotor.h`).
- **Servo**: Rotates an ultrasonic sensor to scan for obstacles.
- **Movement**: The robot can move in all directions and stop.
- **Obstacle Avoidance**: The servo sweeps left and right to check for obstacles, and the car makes decisions to change direction accordingly.

> **Note:** The obstacle avoidance logic must be added to the `loop()` function to make the robot respond to ultrasonic sensor input. The current version demonstrates basic movement and servo rotation.

## 🗂️ Files

- `main.ino` — The Arduino sketch containing:
  - Motor control functions (`moveForward()`, `moveBackward()`, etc.)
  - Servo control functions (`lookLeft()`, `lookRight()`)

## ⚡ Requirements

- Arduino UNO (or compatible)
- Adafruit Motor Shield v1/v2
- 4 DC motors
- Servo motor (SG90 or similar)
- Ultrasonic distance sensor (HC-SR04)
- Jumper wires and chassis

## 🔌 Libraries Used

- [`AFMotor`](https://github.com/adafruit/Adafruit-Motor-Shield-library) — For controlling DC motors via the Motor Shield.
- [`Servo`](https://www.arduino.cc/en/reference/servo) — For controlling the servo motor.

## 🚀 How it Works

1. The robot sets all motors to maximum speed.
2. The servo rotates the ultrasonic sensor to the right and left.
3. The robot can be programmed to decide direction based on the distance readings from the sensor.
4. The `loop()` runs continuously to keep the car moving and checking for obstacles.

## 📝 Future Improvements

✅ Integrate the ultrasonic sensor distance measurement.  
✅ Add decision logic to avoid obstacles automatically.  
✅ Improve turning behavior for smoother navigation.

## 🤝 Contributing

Feel free to fork the repo, make changes, and submit pull requests to improve the obstacle avoidance logic!

## 📷 Demo

![Robot Car](https://photos.google.com/share/AF1QipN2i4ZVfFdH3K3BgBsKOdkoqmV8SAvtCxIP0jd1qWN2EO2h_t6VTKJbjFJeqEVl-g?pli=1&key=V0tPZkZQcTdrRkRWS1BVWWJVS3BpdC1OOG5FbGZn)  
*A simple obstacle-avoiding robot car.*

---

**Happy Building! 🤖✨**
