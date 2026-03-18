# DSP 1 – Theory

## 1(a) Ways to classify a signal:
* **Time:** Continuous-time vs. Discrete-time
* **Amplitude:** Continuous-amplitude vs. Discrete-amplitude
* **Predictability:** Deterministic (exact formula) vs. Random (probabilities)
* **Repetition:** Periodic (repeats) vs. Aperiodic (no pattern)

## 1(b) Mathematical vs. Physical representation:
* **Physical:** The actual real-world phenomenon (e.g., voltage in a wire, soundwaves).
* **Mathematical:** The abstract equation used to model it on paper (e.g., `x(t) = cos(t)`).

## 1(c) Continuous-time, discrete-time, and digital signals:
* **Continuous-time:** Smooth, unbroken time and amplitude. 
  * *Math:* `x(t)`
* **Discrete-time:** Time is sliced into specific steps (sampled), but amplitude can be any exact value. 
  * *Math:* `x[n]`
* **Digital:** Both time and amplitude are restricted to specific steps (sampled and quantized). It's what computers use.

## 1(d) Concept of a system and mathematical representation:
* **Concept:** A process or device that takes an input signal, modifies it, and spits out an output signal.
* **Math:** An operator (like `T`) mapping input to output. 
  * *Example:* `y[n] = T{x[n]}`

## 1(e) Continuous-time vs. Discrete-time systems + examples:
* **Continuous-time system:** Takes continuous inputs, gives continuous outputs. 
  * *Example:* An analog guitar pedal or audio amplifier.
* **Discrete-time system:** Takes discrete inputs, gives discrete outputs. 
  * *Example:* A software algorithm calculating a moving average.

## 1(f) Is a continuous-time system an analog system?
* **Yes.** In practical engineering, the terms are used interchangeably because real-world continuous-time systems (like electrical circuits) also have continuous amplitudes.

## 1(g) Why and where do we need interface systems?
* **Why:** To act as a translator. The real world is continuous (analog), but computers only understand discrete math (digital).
* **Where:** At the boundaries of any digital processing system—connecting the physical sensors/microphones to the computer, and the computer back to physical actuators/speakers.
* **Block Diagram:** `Analog Signal -> [ A/D Converter ] -> Digital Processor -> [ D/A Converter ] -> Analog Signal`

## 1(h) Describe an analog-to-digital (A/D) converter:
* **What it does:** Converts a continuous-time, continuous-amplitude analog signal into a discrete digital signal made of binary numbers.
* **The 3 Steps:**
  1. **Sampling:** Takes snapshots of the signal at specific time intervals.
  2. **Quantization:** Rounds the exact amplitude of that snapshot to the nearest available fixed level.
  3. **Coding:** Turns that rounded level into a binary number (1s and 0s).

## 1(i) Describe a digital-to-analog (D/A) converter:
* **What it does:** The exact opposite of an A/D converter. It takes a stream of discrete digital numbers and reconstructs a continuous analog waveform.
* **How:** It takes the digital values and usually holds them to create a "staircase" voltage, which is then passed through a smoothing filter (low-pass filter) to recreate a fluid, continuous curve.

## 1(j) Practical vs. Ideal Converters:
* **Ideal vs. Practical A/D:** An ideal A/D converter happens instantly and has infinite precision (no rounding errors). A practical A/D introduces "quantization noise" (the error from rounding), has a limited voltage range (it can "clip" if the signal is too loud), and has a slight processing delay.
* **Ideal vs. Practical D/A:** An ideal D/A instantly reconstructs the perfect original analog signal. A practical D/A outputs a slightly distorted signal that requires physical smoothing filters, has limited resolution, and introduces slight electronic noise.

## 1(k) What is signal processing and its forms?
* **What it is:** The mathematical or physical manipulation of a signal to extract information, remove noise, or change its format.
* **Forms & Examples:** 1. **Analog Signal Processing (ASP):** Modifying physical waveforms. *Example:* A traditional FM radio tuner or a vinyl record player's amplifier. 
  2. **Digital Signal Processing (DSP):** Modifying streams of numbers. *Example:* MP3 audio compression or a smartphone camera applying a photo filter.

## 1(l) Describe Analog Signal Processing (ASP):
* **Description:** Processing continuous physical signals directly using electronic components like resistors, capacitors, and op-amps.
* **Simplified Block Diagram:** `Analog Input Signal -> [ Analog Processor ] -> Analog Output Signal`

## 1(m) Describe Digital Signal Processing (DSP):
* **Description:** Processing signals as sequences of discrete numbers using computers, microprocessors, or specialized DSP chips.
* **Simplified Block Diagram:** `Analog Input -> [ A/D Converter ] -> [ Digital Processor ] -> [ D/A Converter ] -> Analog Output`

## 1(n) Why is DSP preferred over ASP? Are there disadvantages?
* **Why it's preferred (Advantages):** * **Perfect Reproducibility:** It relies on math, not physical parts, so it is immune to temperature changes, component aging, or manufacturing tolerances.
  * **Flexibility:** You can completely change the system just by updating the software code, without rewiring hardware.
  * **Complexity:** Can perform highly complex mathematical operations that are impossible to build with physical analog circuits.
* **Disadvantages:**
  * **Hardware Overhead:** Always requires extra A/D and D/A converters.
  * **Speed Limits:** ASP can sometimes handle extremely high-frequency signals (like microwaves) faster and cheaper than the massive computing power required to sample them digitally.
  * **Power Consumption:** Continuously running a microprocessor can use more power than a simple passive analog circuit.
