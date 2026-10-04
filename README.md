# Make: Magazine Article - Reinforcement Learning for Robotics

This repository accompanies the Make: Magazine article covering reinforcement learning (RL) for robotics.

## Train the Agent

Navigate [here](https://colab.research.google.com/github/shawnhymel/make-reinforcement-learning-for-robotics/blob/main/software/make_rl_train_balance_bot.ipynb) to open the Google Colab notebook.

In Google Colab, go to **Runtime > Change runtime type**. Under *Runtime version*, select **2026.07**. Click **Save**. This allows us to use a standard version and pin the library versions (where possible).

Press **shift+enter* to run all of the cells in order. Note that the actual training cells will take some time (about 15 minutes each). Feel free to check the TensorBoard and evaluation video outputs to make sure the robot is balancing.

## Deploy the Agent

Once training is done, open the file browser on the left side of the Colab window. Navigate to *make-reinforcement-learning-for-robotics/output* and download **actor.h**.

Download this repository somewhere on your computer.

Copy **actor.h** and paste it into your local copy of *make-reinforcement-learning-for-robotics/software/balance_bot_arduino*, overwriting the *actor.h* file found there. Open **balance_bot_arduino.ino** in the Arduino IDE.

In *File > Preferences*, add the following URL into the *Additional board manager URLs* field:

```
https://static-cdn.m5stack.com/resource/arduino/package_m5stack_index.json
```

Open the library manager and search for “M5Unified.” Install the M5Unified library.

Upload the sketch to the M5Stack Bala2-Fire robot. Move the robot to a flat surface and watch it balance!

## License

All software in this repository, unless otherwise noted, is licensed under the [Apache-2.0](https://www.apache.org/licenses/LICENSE-2.0) license.