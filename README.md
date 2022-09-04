I am dead set on creating the best QCW DRSSTC that I reasonably can (So, not the size of a building). So, after taking some inspiration from LTT (the name), I went to work.

Here's the plan:

A FPGA or similar based DRSSTC driver

All ultrafast comparators based on the TLV3604DCKR comparator

In Loneocean's QCW DRSSTC, the protection for the async buck converter is not isolated, meaning that the DRSSTC driver isn't isolated from mains (As far as I and some others could tell). So, for that (and for the UVLO for the isolated power supplies), I chose the SFH617A-1 to isolate at a relatively fast speed (as far as optocouplers go)

Gate Drivers - UCC5390ECQDWVRQ1

Modular Primary Capacitors
      -One based on the unobtanium cylindrical mica capacitor
      -One based on some large C0G SMD ceramic capacitors
      -One based on the sketchy Ebay ceramic doorknobs
      -One based on one of the traditional film MMCs
      
Modular Primary Coils
      -Due to the different values that are unavoidable in the modular primary capacitors, separate primary coils would be required to maintain secondary and primary resonance.
      
Inverter - Triple full bridge using FGH75T65SQD-F155 IGBTs

Buck Converter - Either three parallel FGH75T65SQD-F155 IGBTs or an IGBT brick.

Cooling - TBD, may do water cooling :troll:
