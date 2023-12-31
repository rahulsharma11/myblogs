---
title: "Drone building from Scratch with Practical Information"
datePublished: Wed Aug 02 2023 17:39:44 GMT+0000 (Coordinated Universal Time)
cuid: clku0jfpz000009l2cdxbaqfj
slug: drone-building-from-scratch-with-practical-information
tags: drone, ardupilot, mission-planner, qgroundcontrol, quadcopter

---

# <mark>Building Your Drone from Scratch: A Step-by-Step DIY Guide to Crafting Your Dream UAV</mark>

# <mark>Part-1</mark>

Hi there! Welcome to an exciting journey of building your own drone from scratch. I'm Rahul Sharma, a Hardware Design and Computer Vision Engineer. Let's dive into the world of drone-making together!

### **Introduction**

I'll not only provide you with educational content but will also share my personal experiences throughout this journey. So, get ready for some exciting insights!

If you're new to this field, no worries! We'll cover everything you need to know but not in detail otherwise it will be too lengthy:

Feel free to explore the topics according to your interests.🤗

* **Different types of** **drones**: Learn about the various types of drones and their applications in different industries.
    
* **Components for Drone**: Explore the essential components needed to build a functional drone, including motors, propellers, flight controllers, and more.
    
* **Connection Diagram**: Understand how to connect and wire the components together to form a complete drone system.
    
* **Assembly**: Step-by-step guide on physically assembling the drone frame and integrating the components.
    
* **Getting Started**: Learn about the pre-flight preparations, calibration, and safety checks before taking your drone to the skies.
    
* **First Flight**: Experience the thrill of launching your drone for the first time and the basic flight manoeuvres.
    

I hope you find this blog helpful in your journey of drone building. Let's get started!

For more updates and related content, you can visit my [LinkedIn profile](https://www.blogger.com/blog/post/edit/8181348043070001817/4476928216763764192#) and connect with me there.

## Different types of Drone

**Based on Size:**

*1) Nano (Total take-off weight = &lt; 250gm)*

*2) Micro (Total take-off weight = 250gm - 2kg)*

*3) Small (Total Take-off weight = 2kg - 25kg)*

*4) Medium (Total Take-off weight = 25kg - 150kg)*

*5) Large (Total Take-off weight &gt; 150kg)*

**Based on Aircraft type:**

*1) Multirotor Drones*

These are having multiple motors and propellers with a defined structure. Here Propellers are used to generate the lift.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjvIE5WPwytqalSSsYtt2GekAD-t8VRnZAf5Oa1zDjgJm9IwqSPJjv6ZjKRgPTx8O-1PNZv2IvpVjrObBaV6WSfZK423hGO9VtezDd7geT9l9P3u3exBn0l30JtwODy33WB2hPRMf5kmkkfnB22ROgxjSNVDDgZFbTfTTD49VrvDDjS1P6my6Z9JQ1853DP/s1600/multirotor.jpeg align="left")

source-

[https://en.wikipedia.org/wiki/Multirotor](https://en.wikipedia.org/wiki/Multirotor)

*2) Fixed Wings*

These are like Aeroplanes which have fixed wings to generate the lift.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgGZrKfbyoWt0EyQInWb5myPT_kSSFsqKe_RJqdhjTcQ-dAeh-_E1XsEHnrrukDfOlcdE5DpvSptCguue7gwOmZp14DurVh3itmykbZHqM7ap-ioFS4K8N-_rQ_Y3eGT37YH96D_rtR8SKLIBjIWz3MWeye8y_wkTxwE4VAMKNvktidw9Phlh0mtPhrT22m/s320/fixed-wings.webp align="left")

source-

[https://www.indiamart.com/proddetail/fixed-wing-uav-for-aerial-mapping-and-survey-surveillance-8525280348.html](https://www.indiamart.com/proddetail/fixed-wing-uav-for-aerial-mapping-and-survey-surveillance-8525280348.html)

*3) Single Rotor*

It is like Helicopter where single rotor is used to generate the lift and manuavor also. Tail is used to counter the torque generated by one rotor.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEi5zoAnZMTL9Cwmp-Y8D0rMyR0xm4Iyj3krmxzYr8PwCfSUm3b-uQSjk2GE5UYckcqRAIKeOxGactDxgWdi5HPb1TBiR_AIbyI2J4eSdWGFVUaiOILICvqdO6ejizR4GqoSkxO6RJ5GkIw4DL9HR9PPA1nM5bpN7x6_fCT9Jx9XRnUFny6QYHoDU-mH4jia/s320/single-rotor.png align="left")

source-

[https://www.researchgate.net/figure/Single-rotor-drone-image-credit-Velosuavcom\_fig3\_331719966](https://www.researchgate.net/figure/Single-rotor-drone-image-credit-Velosuavcom_fig3_331719966)

*4) Fixed Wing Hybrid VTOL*

These are built for long-range applications. These have both Fixed wings and multiple rotors. These can take off vertically and glide in the air like aeroplanes.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhb6RZUeRpoOEtcSJp6C7gtBFJyOmethC3i3mMSsh00xJMd-uoATu0PqmwFNj4K4X1gKP84ziHZx3PNZwLdQwsnKKtdc2J3gXBI5W4rsc6oC_ByWhTMXtyB_9DCPMPH4KcKvS57zZIFgHX3oXE-9ST96lDgBcsu-pMCJ6TKaSWYW3kx4PC4X4lxUnxa9Zx0/s320/vtol.jpeg align="left")

source-

[https://newatlas.com/carbonix-volanti-vtol-fixed-wing-industrial-uav/48253/](https://newatlas.com/carbonix-volanti-vtol-fixed-wing-industrial-uav/48253/)

### *<mark>Here We Will only Discuss the MultiRotor (Quadcopter).</mark>*

### ***<mark>If you want to learn more about the different types of drones you can comment.</mark>***

## Components for Drone

**\*) BLDC Motors**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjQMpO9DQT6ODAa0vThn0PGrZlhA5mO3WROlEDpaET59QY2kozuc9nNph_iwniOMXe3cHe3Xa5ev9FOv_2Z-0MBqBjhAiVA5fF1yRjoEP0Tp8c-lnWTVzNyusCdxSDaIhBIjFC0au-EHBS_BSYmrv1byXSvt8owXlYkAvCG02JpKzPluwBtwf0FPBK7jhUy/s320/bldc.jpeg align="left")

source-

[https://robotist.in/product/dji-2212-920kv-brushless-dc-motor-for-drone-with-black-cap-cw-motor-rotation/](https://robotist.in/product/dji-2212-920kv-brushless-dc-motor-for-drone-with-black-cap-cw-motor-rotation/)

BLDC motors are generally used for Drones due to their high power, high RPM and low wear and tear.

**\*) Propellers**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiaRtjyFmd5yIVQRtz_Dp1SwHVQq79sJpk0zf37ZybyvmUVc80WSHgN9-9tJHmDNf6KKTL4RKR5E4ONIbxIaxk1za8sJyzztZpLhuhmUmH0Lweg8zSv-90zm1Lh3sVG1dBi7vrb7z3wqomfu8y2SEvRmn3fDkoem10bgJgiwfREmVe2Qq64iMagId64lKUz/s320/props.jpeg align="left")

source -

[http://www.rchyderabad.com/carbon-fiber-rc-timer-propeller-multirotor-drones.html](http://www.rchyderabad.com/carbon-fiber-rc-timer-propeller-multirotor-drones.html)

Propellers are used to generate the required thrust. Choosing the proper propellers is crucial because you have to calculate the Pitch, Diameter for the particular motor. Each motor's property is different hence how much the current motor consumes to make 1 turn and in that turn how much lift is generated directly depends on the Propellers. Choosing the wrong propellers can make the motor hot and can reduce the life of the motor also.

It's better to see the motor specs where it will be mentioned how much thrust it generates with which propellers and at what RPM. Follow that only.

### <mark>Practical Scenario:</mark>

I used T-motor (MN6007), and there were full specs written for this Motor with 22-inch propellers.

I had 20-inch propellers in spare so I used 20-inch one.

After a few iterations, I got to know that to make it lift, I need to give a bit more throttle and when I checked the logs I found that the motor thrust generated was at a bit high RPM than it was mentioned in the specs with 22-inch propellers. So clearly found that although your drone will fly internally you are costing your motor.

**\*) ESCs**

[  
](https://www.blogger.com/blog/post/edit/8181348043070001817/4476928216763764192#)

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiIvc7obKANTlU87jrvwQXPq9agetqiUeaaHnI-7ZZIIit57TBpHG-Nk4_aThA7N5_GLOJU-m9dTKGMc8gKdq-c8xksVMgiEG8ov8tp0ewVP6wS1B6uHUheSMqlOsf-5CX26adnoJcS0YN00kwfRBnVrcacD43E0-In2pdxKmFaw1TJP96ifSwXyIha0uDa/w249-h249/esc1.jpeg align="left")

source-

[https://www.xbotics.in/esc/702-xbotics-40a-esc-2-4s-esc-drone](https://www.xbotics.in/esc/702-xbotics-40a-esc-2-4s-esc-drone)

ESCs (Electronic Speed Controllers)-

These are used to convert the PWM generated by the Flight Controller to generate the 3-phase PWM output that drives the BLDC motor.

**\*) Battery**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjzkGpVdnauPl96HtJNhBOwaED6stPrVIJdBjbjjlzIb1eB9L4gUruVz8YQT6AVVDfTsusV0xjyzYc0TbD3cUP6GtRm7FOmEB5zW1mLdH8l-9V-sBJqwsl3CDG_FMvjz-ei1VRxPV07ghjM8dn0zhJGJybu6HxnTJ320RXmX_C5OK-l7vQJUuH_nfxPH-P_/s320/battery.jpeg align="left")

source-

[https://www.xbotics.in/battery-charger-agriculture-drone/937-tattu-22000mah-6s-25c-lipo-battery-for-drone](https://www.xbotics.in/battery-charger-agriculture-drone/937-tattu-22000mah-6s-25c-lipo-battery-for-drone)

Lipo Batteries are used to provide the necessary power to the System and Drone.

**\*) Radio Telemetry**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjqtwLRY49X64KuvXnhuvgw6EH3vTmJx2ggMi5MqajfEMzUbJCCJGukA3tKoFVT4OvtyUKwgeNMl-nFCQBfak-wdY-n3WDqucttKaxGSasLHM6AJbvJrXqsnGTtFThYd2FTz5vzTvlyInA49XlFkhZba4f3tK0gOKyWprByzbxlzkuDxbZNJpKe0-D7oTfo/s320/telemetry1.jpeg align="left")

source-

[https://www.amazon.in/Tradico-915MHz-433MHz-Telemetry-Android/dp/B07GZVTSQF](https://www.amazon.in/Tradico-915MHz-433MHz-Telemetry-Android/dp/B07GZVTSQF)

Radio Telemetry is very useful for your drone. Although your drone can fly without this but believe me this is one of the useful components for your drone.

This gives the real-time data from the drone to your Ground Control Station which can be monitored to take live decisions. It is also helpful while following the process-

\*) Compass Calibration

\*) Drone tuning

\*) Battery status monitoring

\*) Flight Path and Auto Mission settings and Monitoring and Many more.....

So it's always recommended to use Telemetry with your Drone.

Exception:

These days high-grade Radios are also having this facility but you need to decide on your budget to purchase those Costly Radios.

**\*) RC Radio**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhNwzogdAJd74g_UOVigE1O6A84MypLQOTxIhapN6t2-8bk8c4r8j4Rd2woHuv2HJvVHsK3dV2wVlYBmqQlxNqx-Zi1nnRWNiK8kenfTbmjXk7hSbGRW2w71F1Vb-USbv0b0uzMuonWV_r0S2wb-puaJG4OZSXLN6enrxx2MX3WoNQsQuzbXS3CE_Ozih_J/w399-h399/radio.webp align="left")

source -

[https://robu.in/product/radiolink-at10-2-4ghz-12ch-rc-drone-transmitter/](https://robu.in/product/radiolink-at10-2-4ghz-12ch-rc-drone-transmitter/)

RC Radio is useful to control the Drone remotely. It sends a Radio signal in a particular bandwidth and is interpreted by the RC receiver which is connected to the Flight Controller.

The transmitter sends a signal and the receiver receives the signal. As simple as that. But there are 2 types of Radio one in which the throttle stick is Self-Centered and in another, it is not.

I prefer to use self-centred throttle due to a specific reason. That I will tell you later.

**\*) Flight Controller**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhiadkTCydmScvFAIIzA-D4hVNSQ5MB-fZdHHguzr-ggCo2sOH_IVkmrFkRpzRM63uAegYIR7heIhRrbqp_Srh8nvxCDSg3JyE39i_5SuIGsJkaxXT1HRhfDs0z840GlOMHyHPpyPRWDoGaz55BV-wTwtKE4yWEjlnZqc1cg1h473wThUzlxzUsd5h9aOlX/s320/cube-orange.jpg align="left")

source -

[https://docs.px4.io/main/en/flight\_controller/cubepilot\_cube\_orange.html](https://docs.px4.io/main/en/flight_controller/cubepilot_cube_orange.html)

Flight Controller Pixhawk which is the Brain of the Drone. It consists of advanced sensors like IMUs, Barometers, Compasses and different types of Communication Protocols like CAN, UART, and Serial. This small and powerful board does all the real-time calculations to make the drone fly stable in the Air.

I used the **Cube-Orange Flight** Controller.

**\*) Power Distribution Board**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiiTwyc9PeKHSYfxlqWeJwzrBqapr0LcBlqwMtWv8SepOmd0hN4IF59YYfsT03WR3QZXxvC7nrEYsk02CUH9LCo3ErWdY9fxRk5IEExysc0ZMrOFiuYa_OsqCl3Vox98e8qunqln85KJyfvt59vcgVS3lj70i6NB5f6VU1NhN0vXP7iRXCgL44YDYnSFf5A/s320/pd1.webp align="left")

source-

[https://robu.in/product/multirotor-esc-power-distribution-battery-board-quadcopter/](https://robu.in/product/multirotor-esc-power-distribution-battery-board-quadcopter/)

The power Distribution board is very useful to connect multiple motors terminal at once in a simplified way.

It can also provide regulated power that can be used to actuate different external sensors that are mounted on your drone.

**\*) GPS/Camera**

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg75DWemBfjLOYYMP5onjDcS0qUOaAnijBP6XTAX3DMcLLhCPc0KKIJrHCwyetlbD68Jf4Hnk4JDIYLurh1JVKurQmbN0kCD9YXMm47fkbXS4f29q_mj4yY3PrHPrrmd9L8ZI6mnuPYUsYlW3uGfyuA3mNgY7NzR7sG4i3Qj4KsaJ2O8vT1XC8xU9uSZRXY/s320/gps.jpg align="left")

source-

[https://www.amazon.com/HEX-Here3-GNSS-Module-iStand/dp/B0C3KBK7N4](https://www.amazon.com/HEX-Here3-GNSS-Module-iStand/dp/B0C3KBK7N4)

GPS is a must for the beginner as it is required to fly the drone in Loiter mode or position hold or Alt hold mode.

Without this, you have to fly the drone on your own.

Alternatively, you can use the optical flow camera that gives you a change in X/Y direction which is used to put the drone in a self-hold position.

**\*) Payload (if required)**

These are the extra component which you want to carry along with the drone like camera, lidar etc.

You should tune the drone with the payload to use it effectively.

## Connection Diagram

Straight from the Official page of Ardupilot here is the Connection Diagram attached.

Reference of the image-

[https://ardupilot.org/copter/\_images/Cubepilot\_ecosystem.jpg](https://ardupilot.org/copter/_images/Cubepilot_ecosystem.jpg)

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEirO0tLM2TUGOU31GQm8iGo_58vqLHstSCXGU28sOC-mQwU_NSGEz-1mOLizE7_LBQrb0LQCBjjK4nXn5v-1mpU01OP6PrBFK0kVlHm87a2kThH6lZ6fHcJ6nLBYg-UlR0kTVrirC9wbcDesMSOBZnuKa3MG_BKsqc_TCqYLQy4Ppgw4JE467lrpENN-LpY/w579-h770/Cubepilot_ecosystem.jpg align="left")

As you can see all the necessary connections of ESC, motor, flight controller etc. This is a very good image depicting everything you need to know about the connection.

Still, you want to ask anything related to this, you can comment.

**Assembly**

🔹 **Building the Solid Base Frame:**

The foundation of any successful drone assembly is a robust base frame. If you intend to have landing gears, ensure they are included for smooth landings and to keep the drone stable when at rest. For those constructing foldable drones, pay special attention to the joint connections, ensuring they are sturdy and reliable.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjnFSTBp30_RcryyPy6P0zQmUiCxMPv8olVs20I2-Rb-o2KEU5YThYbBd6eH1Fmd6Mfl5kmBsfKFgfUTulNrLKRDlZUX42tgsifihJcV1U9HS0VZUvvXOpEUZRVqgQ5yMqJzr4sKrRj7ps23jgS7NsMMXOzvzBPhcwT4w1at8isczJY2nniadcje5eS5YEy/s320/drone.jpeg align="left")

I used a T-motor FOC combo that includes Motor+ESC+Propellers.

**🔹 Attaching the Motors to the Arms:**

Securely attach the motors to the designated arms of the drone frame. Double-check that they are firmly fixed in place to prevent any issues during the flight.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj6d7wKNkmHpJeBISqEIE-wtQwI9IR7jtpLAu3HbRw1t53UlWn92puL9jDi6MzOj1eswurKDKd49ILEJzNKhhQhKSNQ8oBfki2nw5WeOpa-G0B6uAxKzyJJytRqCrpBZJtj-6eXtbzWQ8XQIeIvArCxnZD0eaT14nqCfSn0txwj2lP7frCoUIsT5-k6ZJuY/s320/IMG_2928.heic align="left")

**🔹 Fitting the Propellers:**

Refer to the provided diagram to correctly fit the propellers onto the motors. It's essential to understand the proper orientation of each propeller to ensure stable flight. However, refrain from connecting the propellers at this stage, as we will perform ESC calibration before the final attachment.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiBWLhwFZPM8uMjM1mGYrJ0J0KvzF4a-3xanmbMIA6b7Z0mAUeoAbUezx7SiXnzrL3m8pQaJz7SPTh37HpCxaJp6hSzwGMXJ_vo1efCijMIPQ5Gk7sDcs03nfp4jrQy9XB2dmt1W1EDl_jsBa7Ru3dJjRhiEKUUw-zoHdhEzTZP7V7s5pT-UKmQ6PNy58Ac/s320/quad-props.png align="left")

**🔹 Connecting the Motor Wires and ESCs:**

Now, connect the motor wires to the Power Distribution board and the ESC wires to the Flight Controller's Main Servo pins. This step is crucial in establishing the communication between the motors and the flight controller, allowing for precise control during flight.

Connect the 2-pin wire with Flight Controller in Main-servo connectors serially.

Note-

There are combo packs that include all 3 components - Motor+ESC+Propellers which makes it easy to use without any confusion, Those are known as FOC

**🔹 GPS Module Connection:**

If you're using the here3 GPS module, connect it using the CAN1 port designated for GPS connectivity. A properly functioning GPS is vital for accurate positioning and navigation capabilities during flight.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjLP6Fa0ppv03lp6YmrXFOqmNEQdB44vZ4JRwZ6AriQxiSdr6_pS6H6hRzNq6FjXrGNSNsopRZ2xYcV2HxziXdxwmcrBHPCdHzMLnjjrxlztPpk7jglfx6PhKg4aYtkCwBVFAPdJw-2iNKEIc8a4LDDHJ6ZhywII9iuOMVa2ddib6wzcas0_AUGjiL8zDsQ/w548-h387/gps-connection.webp align="left")

source-

[https://docs.cubepilot.org/user-guides/here-3/here-3-manual](https://docs.cubepilot.org/user-guides/here-3/here-3-manual)

This is a very good guide to study to understand different types of connectors and their pin configurations.

**🔹 Radio Telemetry Setup:**

Connect the Radio Telemetry to the designated serial connector on the Pixhawk flight controller. This connection enables communication between the drone and your ground station, providing real-time telemetry data during flights.

Connector - UART1/Serial1 in flight controller board

The above picture also shows the Telemetry connection.

**🔹 Battery Power Module:**

Next, connect the Battery Power Module to the flight controller. A well-configured power supply is essential for a consistent and reliable power source during flight operations.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEg5T2TbGDGwOfgrkJB_tYIet7XwmX7gsGMHIs6TDqWJ3TgR8WjstL20Ro9XxiRHsw3N0Z3G262b5tlnV8NqwvXZDM4TlIwhHQkpfL1afJGCOwfEA_5nzniV5l3c9_uz5ncfelLKFXLLp49vvffVxWg0d2U__VuNYW5PfIJYufzvCENLU8DrK2VOpgt9RqZI/w466-h155/power-module.jpeg align="left")

source-

[https://ardupilot.org/copter/docs/common-3dr-power-module.html](https://ardupilot.org/copter/docs/common-3dr-power-module.html)

**🔹 Leveling Motors with Carbon Fiber Rods:**

If you're using round carbon fiber rods, take the time to level the motors and securely fasten them in place. Properly aligned motors ensure smooth flight and prevent any instability issues during operation. Avoid the temptation to connect the propellers before thoroughly securing the motors to prevent future complications.

![](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj1z7yr2Zueq37BUtmf5vZro8RPspjI8_C7qZtwLau7o0CuKa28JcQ_g_YoOWk73y8e0ygUOEjPV4A3Si6U1_erG0vf3dubdOE8vrLSxSnGtp06ePYba3UfQMhox19m65hMJYAFBjvGDJu-7w488NMVJ8vKYj6mCZ2is1-obDeuCZ46RxrzBG_dgxAOJM1Y/w409-h257/IMG_1607.jpg align="left")

A better way to level is to connect the propellers and place your drone at a horizontal level. Measure the distance from the ground to the tip of the propeller on both sides and make it perfectly the same.

This way you can level the motors easily and most efficiently.

**Practical Scenario - Troubleshooting Rotational Issues:**

In some instances, when your drone is just above the ground and begins rotating either in a clockwise (CW) or counterclockwise (CCW) direction, there are two possible culprits:

***ESC Calibration:***

Firstly, check if the Electronic Speed Controllers (ESCs) are correctly calibrated. ESC calibration is vital in ensuring that all motors spin at the same speed, providing balanced thrust during flight.

***Proper Motor Leveling:***

If ESC calibration doesn't resolve the rotational issue, then examine the motor levelling. Ensure that all motors are level with each other and securely fastened. Misaligned motors can lead to erratic behaviour and instability during flight.

## Getting Started

Once all the connections are done. Then go to an empty open space and do the followings-

**1) Radio Calibration.**

\*) Open Mission Planner on a laptop.

\*) Power on the drone and let the Device be connected (select Buadrate         57600 and /dev/ttyusb) from the top right corner.

\*) Go to the "Mandatory-hardware" tab and then the Radio Calibration option and do the steps that are been asked.

For more reference-

[https://ardupilot.org/copter/docs/common-radio-control-calibration.html](https://ardupilot.org/copter/docs/common-radio-control-calibration.html)

**2) ESC Calibration.**

\*) Remove the propellers before performing ESC calibration.

\*) Go to the ESC calibration section and click on the button.

\*) After that remove the power of the drone and power it again.

\*) After it boots up, you will hear the beep sounds that represent the ESCs calibrated.

\*) You can check the motor rotation for each motor with your stick.

For more reference-

[https://ardupilot.org/plane/docs/common-esc-calibration.html](https://ardupilot.org/plane/docs/common-esc-calibration.html)

**3) Compass Calibration.**

Remember to connect the GPS pointing direction should be the same to as Flight Controller Pointing Direction as both will be oriented in the same direction.

\*) Go to the "Mandatory-hardware " tab and select Compass calibration

\*) Please check your external GPS is displayed there.

\*) Click on Compass Calibration and perform all axis rotations.

\*) It will display the calibrated values after done.

For more reference-

[https://ardupilot.org/copter/docs/common-compass-calibration-in-mission-planner.html](https://ardupilot.org/copter/docs/common-compass-calibration-in-mission-planner.html)

## First Flight

This crucial stage of the setup process requires careful attention to detail to ensure a smooth takeoff and successful flight. In this article, we will provide you with a step-by-step checklist, along with tips and recommendations to make your maiden flight a success.

**🔹 Power On and Check QGroundControl:**

Begin by powering your drone and launching QGroundControl on your laptop. QGroundControl is chosen over Mission Planner for its user-friendly interface and a clear indication of your drone's readiness for flight. As a beginner, it's vital to rely on the software to verify if all sensors are correctly calibrated before takeoff. If the software indicates that your drone is "**Ready to Fly**" you can proceed confidently. Otherwise, carefully review any error messages and address the necessary adjustments.

There can be several issues like-

**EKF related** -&gt; make the drone stable for a few mins to get it rectified automatically.

**GPS Lock** -&gt; Loiter/Alt hold mode will not get used without GPS Lock.

**🔹 Selecting the Right Flight Mode:**

In Ardupilot Software, various flight modes are available, each serving different purposes. While the documentation may suggest starting in Stabilised Mode, i recommend using Loiter Mode for your first flight. This mode provides a more forgiving flight experience, making it easier for beginners to control the drone and execute manoeuvres with greater stability.

### \*\*\*Using Self-Centered stick in Radio Controller\*\*\*

Whenever you are flying a drone, you have to control both sticks in the radio to control the throttle and roll-pitch-yaw of the drone.

For a beginner, it will be difficult to do that and I am sure you will end up crashing your drone.

Hence you need to fly the drone in a way where you don't need to control the throttle and just roll and pitch ("Loiter Mode").

But for Loiter Mode, your stick needs to be in the centre after you armed your drone. Then you can make it fly up/down by moving your throttle stick up from the centre/down from the centre.

Thus if your stick is self-centred, then you just release it after arming and you need not worry about its placement. But if you are using a non-self-centred stick, then you have to manually put it in the middle which needs very preciseness and smooth finger movement.

I hope you got it now why Self-Centered Stick is a better option to use for throttling the drone.

**🔹 Performing the First Flight:**

Once you've selected Loiter Mode, perform a test flight by flying your drone approximately one meter above the ground. Observe its behaviour and stability for a few seconds before initiating a controlled landing. This preliminary flight will allow you to assess if your drone is functioning correctly and if any adjustments are needed.

**🔹 Troubleshooting Motor Rotation:**

If your drone topples in the ROLL or PITCH direction, it may indicate incorrect motor rotation or improperly connected motors. In such a case, double-check the motor rotation directions and correct any incorrect connections.

**🔹 Identifying Leveling Issues:**

Should your drone start rotating excessively in one direction without toppling, it may suggest an imbalance in motor levels. To address this, carefully check and adjust the motors' positioning to ensure a balanced configuration.

**🔹 Calibrating ESCs for Yaw Stability:**

If your drone exhibits undesired rotation in the YAW direction and remains at a specific angle, it indicates an issue with the Electronic Speed Controller (ESCs) calibration. To resolve this, perform an ESC calibration to ensure smooth and stable YAW control.

**🔹 Radio Calibration for Optimal Responsiveness:**

If you notice sluggish response in the ROLL or PITCH direction while your drone reacts quickly in other directions, your radio may require calibration. To rectify this, remove the propellers and recalibrate the radio, ensuring precise and consistent control inputs.

**🔹 Analyzing Flight Logs:**

Once you've safely landed your drone, take the time to review the message logs in the Ground Station. Analyzing these logs will provide valuable insights into your drone's behaviour during the flight. This analysis can help you identify any issues that might have gone unnoticed during the flight and aid in making necessary adjustments for future flights.

***Note*:**

*If you are done with the above steps that is a happy moment but don't think that your Drone is now ready to fly... Tuning is still left and believe me that is very much important before flying a drone repeatedly in Air because if you encountered sudden GUST then your drone should be well-tuned to be stable.*

\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Thank you for joining me on this journey of drone DIY. I hope this comprehensive guide has empowered you to unleash your creativity and passion for drones. Whether you're a seasoned drone enthusiast or a newcomer to the world of UAVs, building your drone is a fulfilling and rewarding experience.

Feel free to share this guide with friends, colleagues, or anyone who might find it helpful.! 🚀🛩️📸

**I am making another blog for the following topics if you want to learn more then be in touch and let me know in the comments.**

***\-&gt; How ESC works and makes the motor run.***

***\-&gt; Drone Tuning.***

***\-&gt;  Payload Integration and tune.***

***\-&gt; Auto Mission.***

***\-&gt; Companion Computer Integration.***

**\-&gt; *Dronecode.***

**\-&gt; *Different types of Propellers and how to choose.***

***\-&gt; Different types of batteries and how to choose.***

Till then Happy Droning😊.

This is my first blog so if there is any mistake in this blog, let me know in the comments...I will be happy to rectify it.

Rahul Sharma

[LinkedIn](https://www.blogger.com/blog/post/edit/8181348043070001817/4476928216763764192#)

#DIYDrones #DroneEnthusiast #UAV #DroneBuilding #DroneTech #DroneLife #DroneCommunity #TechInnovation #DroneLovers #AerialPhotography #DroneFlight #DroneCreators #TechDIY #Makers #TechTrends #AerialAdventures #TechEnthusiast