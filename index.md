## Dumpsys Visualizer

A tool for displaying android dumpsys log graphically in HTML.

**Features**

- Parsing dumpsys log in proto format defined by official AOSP
- Displaying dumpsys log graphically in HTML with a built-in web server

Currently, visualization of the followings are supported:

- `dumpsys activity activities`: Android task stack
- `dumpsys activity processes`: Process state

# Support

| Android          | Support |
| ---              | ---     |
| Pie - 9.0.0_r3   | ✅ |
| Oreo - 8.1.0_r33 | ❌ |

# Next

- **Process dumpsys log more than `dumpsys activity activities`**

    Actually, we can parse other dumpsys log easily, in that they are already supported by [proto/frameworks/base/core/proto/android/server/activitymanagerservice.proto](proto/frameworks/base/core/proto/android/server/activitymanagerservice.proto)

    The most part of work is to design the visualizer of other dumpsys log, such as `dumpsys activity broadcasts`, `dumpsys activity services` etc.

- **Deep integration with manufacturers of smartphones**

    More detailed log is depeneded on root permission and custom features by manufacturers of smartphones.
