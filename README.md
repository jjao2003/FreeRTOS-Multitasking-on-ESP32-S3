Unlike traditional Arduino programs, where everything runs inside the loop(), FreeRTOS allows us to create independent tasks that run concurrently. This means the LED can keep blinking while the counter keeps increasing, without blocking each other.

Why is this important?
Most IoT and embedded applications require multitasking.

With FreeRTOS, we can assign priorities, delays, and resources to different tasks.

The ESP32 has two cores and a built-in scheduler, making it powerful for running multiple tasks at the same time.

In this first lab, you will:

Connect an LED to a safe GPIO pin.

Create two FreeRTOS tasks.

Observe how they run in parallel without interfering with each other.
