---
title: "Танцы с бубном. Зачем нужен Choreographer?"
date: 2023-10-29T18:31:00+03:00
draft: true
---

План статьи:
1. Фрейм, что это такое?
2. Как происходит динамическая отрисовка UI простыми словами.
3. Что такое refreshRate? Почему именно 60Hz и 120Hz? 
4. VSync. Принцип работы. Как применяется в Android?
   1. The HWC generates VSYNC events and sends the events to SurfaceFlinger through the callback:
5. [VsyncEventData](https://cs.android.com/android/platform/superproject/main/+/main:frameworks/base/core/java/android/view/DisplayEventReceiver.java;l=43?q=DisplayEventReceiver)
6. Window, WindowManager, Display
7. SurfaceView, Surface, SurfaceHolder
8. BufferQueue
9. SurfaceFlinger

###  DisplayEventReceiver
Класс, предоставляющий низкоуровневый механизм для приложения, чтобы получить экранные события,
такие как VSync.
