# Full UVM Verification Environment for 16x32 Memory
>This is a UVM-based verification environment to verify the functionality of a 16x32 memory module. This memory module has 16 addressable locations, each with 32-bit wide data. The verification environment will consist of several key components: a testbench >top module, UVM components (agents, sequences, and drivers), and supporting utilities.

🔲 You can see my Repo abou the same Memory module specs and verification Environment without UVM HERE :
>https://github.com/GlassesmanZiad/Full-Verification-Environment-for-16x16-Memory


# 💡 UVM Structure

<p align="center">
  <img width="600"  src="Images/UVM.png"><br>
</p>

## Package1 :
It includes various components like sequence items, sequences, drivers, monitors, and scoreboards, all necessary for a functional verification environment.

This package contains the entire UVM testbench setup. The components within it are organized as follows:

- **Sequence Item Class:** Defines a sequence item that encapsulates the data and constraints for the testbench.
- **Writing Sequence Class:** Defines a sequence for writing data.
- **Read Sequence Class:** Defines a sequence for reading data.
- **Sequencer Class:** Manages the sequence of sequence items.
- **Driver Class:** Drives the sequence items into the DUT (Design Under Test) based on the interface.
- **Monitor Class:**  Monitors the DUT's responses and collects data for analysis.
- **ScoreBoard Class:** Compares expected results with actual results and determines the pass/fail status of the test.
- **Agent Class:** Groups together the sequencer, driver, and monitor to form a cohesive verification agent.
- **Env Class:** Defines the test environment by instantiating the agent, scoreboard, and subscriber.
- **Test Class:** Defines the test that sets up the sequences and starts them.

 
