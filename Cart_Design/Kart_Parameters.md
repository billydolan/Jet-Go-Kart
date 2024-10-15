<h1>Frame</h1>
<p>
    <ol>
        <li>Welded Aluminum tubing</li>
        <li>Cut to shape aluminum or light-weight steel plate for base</li>
        <li>10 gallon fuel tank spot, with shielding if possible</li>
        <li>Fire extinguisher mount</li>
        <li>Lightweight bucket seat (probably get off FB marketplace or find one in a scrapyard, TBD)</li>
        <li>Multi-point harness, at minimum 3 point, if not 5 point</li>
        <li>Steering wheel, column</li>
        <li>Axles and rims</li>
        <li>Keep low to the ground and potentially will need a spoiler for dual turbines, or if a certain height is not attainable</li>
        <li>Some sort of smaller shocks at least for handling bumps, potential instabilities, etc.</li>
        <li><em>Roll cage?</em></li>
        <li>Front splitter</li>
    </ol>
</p>

<h1>Wheels</h1>
<ul>
    <li>Disc brakes, all 4 wheels</li>
    <li>Could potentially use brakes similar to a higher performance bicycle, using mineral oil</li>
    <ul>
        <li>Otherwise investigate hydraulics, etc.</li>
    </ul>
    <li>Air holding tires instead of solid rubber most likely → TBD</li>
    <li>Guards/fenders on the frame to protect the tires</li>
    <li>Proper brake lines connected to the brake pedal</li>
</ul>

<h1>Personal Equipment</h1>
<ul>
    <li>Helmet</li>
    <li>Fire-resistant or proof suit/clothing</li>
    <li>Some sort of neck brace, especially for dual turbine build</li>
    <li>Microphone in helmet or earbuds</li>
</ul>

<h1>Fuel</h1>
<ul>
    <li>Can be changed, but for single operation, 5-10 gallons minimum</li>
    <li>T-Slot framing to hold the tank in place</li>
    <li>Fuel lines diameter: <em>Fill in later</em></li>
    <li>Kerosene, with JetCat anti-static oil mix</li>
    <ul>
        <li>Price per gallon: </li>
    </ul>
</ul>

<h1>Turbine Mounts</h1>
<ul>
    <li>Machined aluminum mounts</li>
    <li>Three bolts for each side of a turbine</li>
    <li>Put a shield behind the driver in form of a steel plate</li>
    <li>For 2 turbine operation, common electronics config, but separate fuel tanks and mounts on either side of the driver?</li>
</ul>

<h1>Turbine</h1>
<ul>
    <li>Current V1 model would use 1 JetCat P300-Pro with integrated electronics, providing 300N, ~67 lbf at stock</li>
    <ul>
        <li>V2 would use twin JetCat P300-Pros</li>
        <ul>
            <li>Will need to redesign the app to handle 1 & 2 turbine operational modes</li>
        </ul>
    </ul>
    <li>JET NETS MUST BE USED</li>
</ul>

<h1>Initial Turbine Modifications</h1>
<ul>
    <li>Start with modifying the nozzle to optimize base level thrust</li>
    <li>Weight reduction for the nozzle if possible</li>
    <li>Create a more optimized inlet or cowl to improve intake</li>
    <ul>
        <li>These could be scoops or similar to cars that directs air into the turbine</li>
    </ul>
</ul>

<h1>Complex Turbine Modifications</h1>
<ul>
    <li>Afterburner design, testing, and use</li>
    <ul>
        <li>Create an afterburner that can be as efficient as possible (an ironic statement but possible)</li>
    </ul>
    <li>A turbofan adaptation with proper ducting feeding into afterburner for higher oxygenation of the flow → easier to burn</li>
    <ul>
        <li>Component matching calculations and blade design for the current shaft</li>
        <li>Manufacturing would be costly</li>
        <li>Testing to validate the risk of surge is minimal, in reality needing to be non-existent will be difficult if numerical models are not very fine-tuned</li>
    </ul>
    <li>Combustor optimization for efficiency and output</li>
    <ul>
        <li>Expensive to manufacture</li>
        <li>Modeling software even available?</li>
        <ul>
            <li>Can do calculations using resources from my combustion classes, Cantera, and CEA in Matlab (CEAM)</li>
            <li>Time consuming and very complex, especially for creating entirely new combustors, no matter the size reduction</li>
            <li>Papers available to assist with this, but anything like code will likely not be able to be obtained</li>
        </ul>
    </ul>
</ul>

<h1>Electronics</h1>
<ul>
    <li>An integrated controller with either an interface for changing thrust on the steering wheel, like paddles, or connected to a gas pedal</li>
    <ul>
        <li>Some sort of touch sensor that drops the turbine(s) to idle thrust, then shut off, if not interacted with in a certain period of time</li>
        <ul>
            <li>Will need a way to work around this for idle periods, especially during testing</li>
            <li>Use a button or switch</li>
        </ul>
        <li>Pedal method would require a sensor and tension to take into account the pressure applied to the pedal</li>
    </ul>
    <li>Could work on custom ECU to replace JetCat ECU-Software and run only my own, TBD</li>
    <ul>
        <li>This would need to be heavily documented, no guessing games</li>
        <li>Integrated screen on the wheel, displaying fuel consumption, rpm, etc.</li>
        <li>Raspberry Pi and some sort of screen or simple tablet with a Pi like I saw years ago at Zin Tech</li>
    </ul>
    <li>Speedometer</li>
</ul>

<h1>'JetOp' Modifications</h1>
<ul>
    <li>Need to get displays of values for operation</li>
    <ul>
        <li>Uni CS Senior-project may solve this, at least at the base level</li>
    </ul>
    <li>Ability to utilize commands and functions for multiple turbines</li>
    <ul>
        <li>Some sort of input based on detecting how many turbines are connected, etc.?</li>
        <li>Automatic app behavior changes</li>
        <li>Need to find how to properly display each turbine's performance</li>
        <li>Simplify charts to tachometers and bars only, no need for airspeed</li>
        <li>Split screen setup with the Pi?</li>
    </ul>
</ul>

<h1>Documentation</h1>
<ul>
    <li>Create this as a markdown document at some point, could add to ReadMe with a license for use at own risk, etc.</li>
    <ul>
        <li>Code will be as is, and the timeline is whatever I define it as</li>
    </ul>
    <li>Create a Gantt chart or similar that could be integrated into the portfolio, or on the repository for the Jet go-kart</li>
    <ul>
        <li>Otherwise, use a PNG of an Excel Gantt chart</li>
    </ul>
    <li>Cite sources and provide background for documentation/calculations, especially for things like cycle analysis, etc.</li>
    <ul>
        <li>Logic behind methods taken, textbooks/sites used, etc.</li>
    </ul>
    <li>Propulsion resources</li>
    <ul>
        <li>Textbooks, online examples, videos, etc., will need to be listed</li>
    </ul>
    <li>Create a flow chart for parts of the projects</li>
    <ul>
        <li>Why the selected path, and what the upcoming steps are / what steps have been</li>
    </ul>
    <li>Project updates on a schedule of weekly or monthly?</li>
    <ul>
        <li>Hammer out a simple format, can be posted on GitHub and socials</li>
    </ul>
    <li>Social media documentation through:</li>
    <ul>
        <li>Instagram: bdsprojects</li>
        <li>YouTube: TBD</li>
    </ul>
</ul>

<h1>Software (Will be added to over time)</h1>
<ul>
    <li>Visual Studio Code (VS Code)</li>
    <ul>
        <li>Python</li>
        <li>C++</li>
        <li>C#</li>
    </ul>
    <li>Arduino IDE</li>
    <li>Visual Studio Community</li>
    <ul>
        <li>Compiling:</li>
        <ul>
            <li>C++</li>
            <li>C#</li>
        </ul>
    </ul>
    <li>MATLAB</li>
    <ul>
        <li>Mathworks own MATLAB software & IDE</li>
    </ul>
    <li>SolidWorks</li>
    <ul>
        <li>3D modeling</li>
        <li>Decent fidelity simulations</li>
        <ul>
            <li>Fluids</li>
            <li>Thermal</li>
            <li>Stress</li>
        </ul>
    </ul>
    <li>Converge CFD</li>
    <ul>
        <li>Flow simulations</li>
    </ul>
    <li>Power BI</li>
    <ul>
        <li>Data visualization and or Gantt chart</li>
    </ul>
    <li>Excel</li>
    <ul>
        <li>Potential Gantt chart</li>
    </ul>
</ul>
