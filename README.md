# Chiplet-Die-to-Die-Link-Controller
The task is to implement the control portion of a simplified die-to-die link controller representative of the link management logic used in modern chiplet based SoCs.

As a learning project, I will follow these chunks to manage the project efficiently.  

### Phase 1 | Understand the Design

- [ ] Learn what a chiplet die to die link controller does.
- [ ] Learn the difference between the link controller and the physical layer.
- [ ] Learn the purpose of link initialization and link training.
- [ ] Learn the concept of `ready/valid` handshaking.
- [ ] Learn how link errors can trigger recovery.
- [ ] Learn the three block SystemVerilog FSM structure.

### Phase 2 | Define the Architecture
- [ ] Define the states required by the controller.
- [ ] Draw the FSM state transition diagram.
- [ ] Define what each state does.
- [ ] Define the transition condition for each state.
- [ ] Define the behavior of `link_up`.
- [ ] Define the behavior of `link_error`.
- [ ] Define the behavior of `tx_valid`.
- [ ] Write the complete interface specification.

### Phase 3 | Build the RTL
- [ ] Create the SystemVerilog module.
- [ ] Create the state enumeration.
- [ ] Create the state register using `always_ff`.
- [ ] Create the next state logic using `always_comb`.
- [ ] Create the output logic using `always_comb`.
- [ ] Implement reset behavior.
- [ ] Implement link enable behavior.
- [ ] Implement link initialization.
- [ ] Implement remote readiness detection.
- [ ] Implement link up behavior.
- [ ] Implement transmit control.
- [ ] Implement receive error detection.
- [ ] Implement recovery behavior.
- [ ] Implement illegal state recovery.

### Phase 4 | Build the Testbench
- [ ] Create the testbench.
- [ ] Create the clock generation.
- [ ] Create the reset sequence.
- [ ] Create the normal initialization test.
- [ ] Create the delayed remote readiness test.
- [ ] Create the link failure test.
- [ ] Create the reset during initialization test.
- [ ] Create the recovery test.
- [ ] Create the illegal state test.
- [ ] Add self checking to the testbench.

### Phase 5 | Add Assertions
- [ ] Learn SystemVerilog concurrent assertions.
- [ ] Create an assertion that reset places the controller in the reset state.
- [ ] Create an assertion that `link_up` only occurs when the link is operational.
- [ ] Create an assertion that an RX error causes recovery.
- [ ] Create an assertion for the transmit handshake.
- [ ] Run the assertions with the testbench.

### Phase 6 | Simulation
- [ ] Compile the RTL and testbench.
- [ ] Run the normal initialization simulation.
- [ ] Run the delayed readiness simulation.
- [ ] Run the failure and recovery simulation.
- [ ] Run the reset simulation.
- [ ] Inspect the waveforms.
- [ ] Capture the important waveforms.

### Phase 7 | Synthesis
- [ ] Learn the basic Yosys synthesis flow.
- [ ] Create the synthesis script.
- [ ] Synthesize the controller.
- [ ] Check for synthesis errors and warnings.
- [ ] Record the cell statistics.
- [ ] Generate the synthesized netlist.

### Phase 8 | Static Timing Analysis
- [ ] Learn basic SDC clock constraints.
- [ ] Create a 500 MHz clock constraint.
- [ ] Set the clock period to 2.0 ns.
- [ ] Create the basic input/output timing constraints.
- [ ] Run OpenSTA.
- [ ] Check for unconstrained paths.
- [ ] Identify the critical setup path.
- [ ] Record setup slack.
- [ ] Record critical path delay.

### Phase 9 | Engineering Documentation
- [ ] Document the design requirements.
- [ ] Document the architecture.
- [ ] Document the FSM.
- [ ] Document the verification strategy.
- [ ] Document the simulation results.
- [ ] Document the synthesis results.
- [ ] Document the STA results.
- [ ] Write the engineering notes.
- [ ] Create the final README.
- [ ] Review the complete project as if it were an RTL assignment handed to an intern.
