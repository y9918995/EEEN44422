# 1.1 Overcurrent Protection – Grading By Time  
  
--LECTURER:  
Hello.  
I'm Peter Crossley.  
I'm Professor of Power Systems at the University of Manchester, and Director of the EPSRC Centre for Doctoral Training in Power Networks.  
I am returning to my subject area of Power System Protection and this talk will be about overcurrent protection.  
The first lecture today is about principles of overcurrent protection.  
So when you look at a network of overcurrent relays, the issue is the word coordination.  
How do you coordinate a relay that's located at, for example, circuit breaker one to the relay that is located at circuit breaker six, to the relay that is located at circuit breaker nine?  
If we look at that diagram there, you can see that if the fault is located on line A, it should be cleared by relay one.  
And under those conditions, all of the relays on that network should remain stable and inoperative.  
If you have a fault on feeder F, it should be cleared by the relay located at six.  
And all other relays should remain stable.  
So effectively we're tripping...  
But if that fault was to occur on feeder F, then the tripping of circuit breaker six would disconnect the supply to all the consumers that are connected to the busbar effectively supplying A, B and C.  
And then the loads connected to feeders A, B and C.  
An assumption in that diagram is this is a radio system.  
So the power is flowing from the top, which is assumed to be the grid supply point.  
So when you see the busbar located at breaker nine, this is the grid supply point to this part of this network.  
In the case normally in Britain, that would be an 11 kilovolt radio distribution network.  
So the power flows from the 33 to 11kV transformers into the 11kV network, and down to the consumers which are connected, generally, through 11kV to 400 volt transformers.  
If, for some reason, a fault did occur on feeder A...  
..and if, for some reason, relay one failed to clear a fault, then relay six must operate and must clear the fault.  
So similarly, backup protection for two and three...  
so for circuits two and three, is of course circuit breaker six.  
And the backup protection to circuits four, five and six is nine.  
But, of course if there was a fault on feeder D and circuit breaker four failed to open, it would have to be cleared by circuit breaker located at nine on feeder J.  
And this would, of course, cause a major disruption to the network.  
As a simple technique for all the current grading, is referred to by a Discrimination of Time.  
In this simple diagram I've assumed that the grading margin, which we will discuss in considerable detail later in the lecture, is 0.3 seconds.  
So 300 milliseconds.  
And effectively, when you look at that network, you can see the furthest downstream point.  
I've assumed that the faults had cleared in 100 milliseconds.  
So if, for example, we look at the lowest point on that diagram.  
So then of course what we've got is that the fault...  
So the protection operates at 0.1 seconds.  
As we move up the network, we can see that the next protection relay operates in 0.4.  
As we move to the next level on that network, we can see it becomes 0.7.  
As we move to the next level along the network...  
so this is the circuit breaker linked to busbar F.  
Sorry, linked to feeder F.  
So then it will operate in 1 second.  
And then if we moved up to feeder J, where the circuit breakers now would operate in 1.3 seconds.  
You're beginning to see the advantages and the disadvantages.  
The main advantage is simplicity.  
The upstream relays backup the downstream relays.  
But, of course, the disadvantage is that the longest fault clearance time occurs for faults that are located near the source.  
So if you look...if you'll have a fault on the top transformer.  
So this is perhaps for a transformer from the 33kV system to 11kV system.  
If a fault was to occur on the 33kV side of that transformer, its operation time would be 1.6 seconds in that diagram.  
And, of course, the thing to remember is the fault current is highest for faults that are located closest to the source.  
And, of course, this is a point where the operating time is the slowest.  
So in many ways it's the wrong answer.  
We would like faults to be cleared rapidly if the fault current is high.  
But this is a very simple protection technique using time.  
Later on we'll look at the use of current and time together and you'll see how we've solved some of the limitations of this protection technique.  
This is showing that diagram in a slightly different way of how we begin to think about grading.  
I've deliberately picked an oversimplified case.  
I have assumed that the fuse will operate in 0.1 seconds if the fault current is greater than about twice the fuse rating.  
So if, for example, the fuse was set at 100 amps, if you had a current of 200 amps, it would operate in 0.1 seconds.  
As you obviously realise from my earlier lectures on fuses, fuses have an extremely inverse characteristic, which means that at high fault currents fuses operate very quickly.  
But at low fault currents, which you of course grade to move few setting values, they take a long time to operate.  
But I have assumed that at twice the fuse rating value the fuse operates in 100 milliseconds.  
And if the current is less than twice the fuse rating, it would take an infinite time and it will never operate.  
The next challenge is the down-stream relay must be set above the maximum load currents.  
So when we look at the diagram, the down-stream relay has been set with a time of 0.4 seconds.  
And its setting value must be above the maximum load current.  
As I've shown in my diagram, it's probably been set at about 20 percent above the maximum downstream load current.  
In a sense, it should also be set above the...  
it should clear the lowest current fault on that network.  
In fact, that relay with a 0.4 seconds operating time is protecting both the high voltage side of a transformer, as well as the low voltage side of a transformer.  
So in that diagram you perhaps would assume that the high voltage side 11kV, and then the lower voltage side, 400v.  
And the protection has to see a fault on the high voltage terminals of a transformer, as well as on the low voltage terminals of a transformer.  
That can be quite a difficult challenge, because of course the fault current on the low voltage side may not be very significant.  
But I've assumed that we could set it for 0.4 seconds time, with a current magnitude greater than the downstream relay maximum load current.  
As we now move up to feeder A and the upstream relay, so this is getting closer and closer to the source, the upstream relay has an operating time of 0.7 seconds, or 700 milliseconds.  
'Cause we've gotta either assume the grading margin from fused relay is 300 milliseconds.  
The grading margin between the downstream relay and the upstream relay is 300 milliseconds.  
And then the upstream relay must be set above the maximum load current.  
We do not want protection to operate on load current or inrush current related to the switching on of loads.  
Protection must operate for short circuit faults.  
  
  
  
# 1.2 Overcurrent Protection – Grading By Current  
-- LECTURER:  
I'm now going to look at a more complex network.  
So I'm going to look at a network where we've got a source supply which is coming from that 11kV source.  
It's got a stated range of a 130MVA-250MVA.  
What that actually means is the fault level, that is from 130MVA-250MVA.  
When it's a 130MVA, it means there's a single transformer supplying the 11kV busbar.  
In the case of it being a 250MVA fault level, there's two transformers.  
In the British system when we're going from say, 33kV-11kV, we would normally put two parallel transformers.  
And each transformer is loaded to a level where one transformer could supply all the power.  
So if for example, we've where that source is shown, we could have one transformer or two transformers.  
But the system will still operate correctly when one transformer is out of service which could be a failure or of course it's more likely a maintenance.  
Then of course we have a cable system which is 2km of 240mm² paper insulated cable.  
So I've assumed a very traditional system.  
But it's 2km of cable, of course the protection is located for the cable at busbar J.  
When you look at the network, you realise that the only source of a network is at busbar J.  
And then what we're trying to do for the relay at busbar J is to protect for fault on the cable between J and H.  
So in fact, we have shown a fault at F1.  
Busbar H we now have three cables leaving busbar H.  
We're showing in detail one cable which just consists of 200m of 120mm² paper insulated cable.  
And that is supplying the transformer, 4MVA, 11/3.3kV transformer with a leakage reactant of 7%.  
The protection at busbar H on that particular cable transformer must be able to see a fault F too.  
The fault at the...the fault at busbar G.  
So in fact you must be able to see 3.3kV terminals of the transformer.  
Then of course we go to busbar G and that's moving down to the next bottom network.  
So when we look at that network, we begin to investigate discrimination by using current so grading by the use of current.  
And of course, we're taking advantage of the fact that the expected fault current will reduce as we move away from the source on the network.  
We can of course set relays to only trip now if the fault current exceeds the value expected for their section of a network.  
So we're using the magnitude of a fault current to decide how a protection performs.  
An assumption behind this is we need a reasonable value of impedance between the breaker locations to achieve the grading.  
Where we have a transformer, we generally have a significant value of impedance.  
But where we just have short lamps of line, the impedance change...the impedance is quite small.  
Therefore, the fault currents change can be small.  
And now in this diagram, we're beginning to study the parameters and break down that network.  
So the source when it's a 250MVA source, you remember from your previous lectures what you do is kV² ÷ MVA.  
So you've got 11kV² ÷ 250MVA and you get an impedance value of 0.485Ω.  
When the infeed, the fault level is a 130MVA, it's kV² ÷ 130MVA.  
And we have an impedance value of 0.931Ω.  
Then we have 2km of 240mm² paper insulated cables then we have a 200m of 1200mm² paper insulated cables.  
Then we have the impedance value of a transformer.  
Impedance value of a transformer is 0.07 × kV² ÷ MVA.  
So it's in fact the unit value of the transformer × kV² ÷ MVA which gives a value for that transformer of 2.12Ω.  
So you can see of the transformer from 11kV to 3.3 kV is the high impedance on the network.  
When we do the analysis, we can see at busbar J so busbar J, the fault level...  
Sorry, the fault current when the short circuit capacity is 130MVA is 6.8kA.  
When the short circuit capacity of the source is 250MVA, the fault current is 13.1kA.  
If you put a three phase and all these are for three phase solid faults.  
If you put a three phase solid fault on busbar H and fault current is 5.4kA when the short circuit capacity is 130MVA.  
It's 8.8kA when the short circuit capacity is 250MVA.  
If now we look at the 11kV side of the transformer, I express about because it's very important from a protection point of view to understand what the fault currents are at the side of the transformer.  
So the 11kV side of the transformer when the short circuit capacity was 130MVA, the fault current is 5.2kA.  
A 250MVA, it's a 8.3kA.  
When you look for three phase fault on busbar J, the fault current is 1.9kA when the short circuit capacity of the source is 130MVA and it's 2.2kA at 250MVA.  
When you look through that network, you're seeing how the currents are changing throughout the system.  
When I express busbar G, I deliberately expressed that as if I was in the 11kV system.  
And of course what I'm interested in is the behaviour of the 11kV system.  
And the grading of the protection at J and H with G.  
This diagram showing the change of the fault current as we move through the network.  
So as I mentioned that as you move down the network or downstream, so of course the highest fault current is seen at busbar J, the upstream point.  
The highest fault current is seen when the fault...when the short circuit capacity of the source at busbar J is 250MVA.  
And as we move from J to H, there's a slow reduction in the fault current.  
Then as we move from busbar H to busbar G, there's a large change in fault current because of the transformer.  
What I'm now beginning to look at is how do we protect that.  
I've made an assumption that I've said that the protection is located at busbar G.  
So the relay that's controlling the circuit maker, affecting on the line connects to busbar G has an operating time of 1s.  
Therefore, if we do it purely on time grading and we put 0.3s as a grading margin, the operating time for the circuit for the relay located on the brake connects to busbar H is 1.3s.  
The operating time for the relay located on the circuit brake connects to busbar J is 1.6s.  
These are long operating times.  
If you think about the fault near the incoming source from the busbar J, this is a long operating time.  
So what we begin to think about is wherever we could set a high set all the current element located at busbar H and busbar J.  
So when we look at this, the 5kA, the high set relay has been set with an operating current setting of 5kA.  
It will only operate if fault current is above 5kA.  
So for relay H, we can now set that to a 100ms operation because actually any fault beyond busbar G, will always bear to law current than 5kA.  
Because we can set the relay at busbar H to 100ms operating time.  
We can set the relay at busbar J to 400ms operating time.  
So we're really mixing now these low set overcurrent protection with high set overcurrent protection.  
This next diagram is showing that behaviour.  
So you can see for a relay set at...  
relay G is assumed to be set at 1kA.  
The low set element of relay H is set at perhaps 1.2kA with a gradient margin of 0.3s and then the low set element at J is set to up to 1.4kA with a time operation of 1.6s.  
You can see that those lines do not cross.  
It's very important in a grading study the lines do not cross.  
But of course when we look at that, we realise when we get to high fault current, the fault current greater than 5kA.  
Our operating times especially for the relay at busbar J is very slow.  
Therefore, we put these high set elements.  
The high set elements at busbar H has an operating time of a 100ms and the high set element at busbar J has an operating time of 0.4s.  
  
  
# 1.3 Protection using Fuses  
--LECTURER:  
Hello, I'm Peter Crossley.  
I'm Professor of Power Systems at the University of Manchester and the Director of EPSRC for Doctoral Training in Power Networks.  
The course I'm giving you is related to power system protection and this lecture is specifically about overcurrent protection and the protection of low voltage and high voltage networks using fuses.  
I'm gonna start by talking about overcurrent protection using fuses.  
Fuses were the first type of protection, they were first developed at the end of the 19th century.  
And they're still very widely used today.  
If you think of the electrical system in your home, you have the supply fuse, which comes into your house, which is probably an 80 amp or 100 amp fuse.  
Then you have your consumer unit, which consist of 15 amp, 32 amp fuses.  
Then you have the fuses in your plugs, perhaps one amp, five amp, 13 amp fuses.  
So our world is full fuses.  
So huge numbers are still being used, mainly on low voltage networks.  
They're simple and they're relatively low cost.  
But obviously when a fuse blows it must be replaced.  
The principle of a fuse is that you have conducting material with a cross-section that's incapable of carrying a fault current.  
So effectively you have a piece of silver which is of a thickness, which cannot carry fault current but can carry the load current.  
And normally as you move to high rupturing capacity fuses, you have one or more current carrying elements.  
And during an overcurrent these elements melt and then you get arcing across for breaks.  
When this occurs you have rapid interruption of a fault current and what that's doing is limiting the energy the fuse passes to the equipment which you're protecting.  
So if you think about a cable system, the fuse will blow before the cable is damaged.  
And that is the heart of protection but the fuse is there to protect the component you're protecting.  
So when you look at this diagram of a fuse, you can see what you have is a classical high rupturing capacity fuse where the fact you have the end caps and the connecting strips of the cables and then you have the silver element with the notches in.  
This is surrounded by silica, effectively sand and of course when you get an arc, the sand becomes glassified.  
And then, of course, the fuse is protected within a ceramic holder to prevent an explosion.  
This is showing you more detail, the structure of a fuse.  
So we have the end contacts, we have the core of the fuse where effectively we have the silver elements which are a conductor for current.  
And these are surrounded by silica sand and then we have a protecting glass epoxy tube which is there to protect the surrounding areas.  
So to stop the molten silver and hot sand spreading out.  
What happens on the normal operating conditions, the thermal energy that's entering the fuse is basically being dissipated by the fuse.  
So there's an equilibrium exists and the energy you're putting into the fuse due to the current passing through the resistance of the fuse is dissipated by the heat leaving the fuse.  
But as you increase the current, so as you get effectively a fault current there's a very high value of current flowing.  
The temperature produced by the current exceeds the heat you can extract from the fuse.  
So at this point the elements begin to melt.  
And when you look at the first diagram the elements are melting and you're beginning to get multiple arcs across the nix of the fuse.  
And as this heating continues you begin to melt the sand, you begin to get glassification of the sand, of course the sand absorbs the heat and then what happens is the sand effectively stops the current flowing.  
So on a current zero, the arc is extinguished and effectively the conduction process stops.  
So at that point, the fuse is blown and hopefully the equipment you're protecting has not been damaged.  
The next slide is showing a 3.3 kilovolt fuse.  
So what we've got is the bottom contact, the top contact and then we've got the silver elements with which is where the current passes through.  
And you've got the arcing rod which is where the arc process begins this is all surrounded by boric acid.  
In this particular case there's an expulsion fuse, so it's controlled by a spring.  
And as the silver element begins to melt, the spring process effectively causes the fuse to break the arc.  
The next diagram is really showing this process.  
So in this one the elements are beginning to melt, the silver is getting very hot, it's beginning to stretch then, of course, the spring is then pulling the arc apart.  
At this point, we're beginning to elongate the arc, we start the process of vaporising the boric acid.  
And then the vapour from the boric acid in the final slide begins to quench the arc and at the next effect at current zero the fuse stops conducting.  
So the thing to remember about a fuse is that a fuse elements melt and vaporise when the current is above a set value for a certain period of time.  
The higher it is above the set value the faster it will operate.  
So if you think of a 200 amp fuse, if you've only got 400 amps flowing through that fuse it will take a long time for it to operate.  
However, if you put 4,000 amps through that fuse it will operate in a fraction of a cycle.  
When the process begins, the fuse elements begin to melt and then we start the process of vaporisation.  
At that point you begin to get arcs within the fuse and these have to be extinguished to complete the interruption process.  
So the operating time of a fuse consists of pre-arcing time and the arcing period.  
The pre-arcing time is the period when the conducting silver is beginning to melt and the arcing period is where it is melted, broken and you've got an arc established.  
IEC defines some values, one of them is called the fusing factor, this is the minimum fusing current divided by the current rating and is defined to be 1.4.  
So if you have a 20 amp fuse, the minimum current it will operate for is 28 amps.  
The behaviour of a fuse also depends on the temperature rise of a fuse and how a fuse is mounted within the electrical system.  
And there are of course, standards to define how you mount fuses within an electrical low voltage system.  
Then of course, we have to consider the breaking capacity of a fuse.  
The breaking capacity is the ability of the fuse to break a particular value fault current.  
If you use a fuse which is incapable of breaking the fault current, what will happen is as the fuse tries to break the fault current it will overheat and will possibly explode.  
So obviously every fuse must capable of breaking the fault current that's seen at that point on the power network.  
When you look at these factors, a fusing factor, temperature rise, breaking capacity all these factors depend on each other.  
And the critical climate of a fuse is the energy it lets through into the components it's protecting.  
And the energy let through is determined by an I squared T value.  
So when you think of a cable you're protecting of a transformer you're protecting, this has a thermal withstand capability described by the I square T characteristic.  
And the fuse must blow and disconnect the fault current before the equipment you're protecting is damaged.  
So before the cable is damaged, before the transformer is damaged.  
So it must not let a value of I squared T through greater than the withstand capability of the equipment you're protecting.  
So fuse elements are resistive, hence a fuse absorbs electrical power when it carries current.  
If that current value is constant below the a particular value so effectively below the setting of the fuse or below the operating value of the fuse.  
The power that's entering the fuse, the input power, is dissipated to the surroundings.  
And you have a state of equilibrium, so the energy you're putting into the fuse is extracted from the fuse and the fuse doesn't melt.  
If now we increase the current above a particular value, then a new equilibrium cannot be achieved.  
So we're putting more power into the fuse from we're able to dissipate from the fuse.  
And at this point the fuse elements get hotter, they begin to melt and then as they melt they begin to break, and then as they break they begin to establish the arcs.  
And then this circuit interruption process begins.  
The pre-arcing period refers to the interruption before the establishment of an arc.  
The critical thing to remember is that once a fuse has got to the end of it's pre-arcing period, it has not yet interrupted the current but it is incapable of recovery.  
The fuse is effectively blown but it hasn't yet put out the arc.  
So the pre-arcing period is time from the current exceeding a critical value until the point of melting and the initial vaporisation of the elements.  
And then when we think about the arcing period, this is a time we require to go from where the fuse elements have effectively broken but the arc has not been interrupted.  
So the arcing period is the time to interrupt the arc current.  
This is showing the characteristics of a pre-arcing time.  
So that diagram there is showing the pre-arcing time in seconds for different types of fuses.  
So we have 25Amp fuses up to 180Amp fuse.  
When you look at those characteristics and if we first look at the 25Amps of a 25 LET fuse, look at the characteristics, you can see that the current of 40Amps, the pre-arcing time is 200 seconds.  
So it takes 200 seconds for the fuse to effectively melt.  
If we now increase smart current to 60Amps, remember this is a 25Amp fuse at 60Amps for pre-arcing time reduces to 0.6 of a seconds, so 600 milliseconds.  
If we increase it to 100Amps which of course is four times the 25Amp fuse value then the pre-arcing time is four milliseconds.  
If we're to increase it to 200Amps our pre-arcing time is less than one second.  
Just continuing that process, just to make sure you understand these inverse time characteristics or these extremely inverse time characteristics.  
If we look at the 80Amp fuse you can see that for 160Amps the pre-arcing time of the fuse is 30 seconds.  
If you were to move that or to you to move up a current value to the 200Amps this is the perspective Amperes in OMS.  
This is what would be the current fuse did not blow.  
On a 200Amp you would now have a pre-arcing time of five seconds.  
If we increased it to 400Amps, the fuse will operate in a quarter of the cycle.  
So the fuse would the fuse for pre-arcing time of a fuse would be five milliseconds.  
So just repeating this again, the greater the current is above a maximum value at which equilibrium is achieved the shorter the time before melting.  
So at very high current values fuses into the current very quickly.  
At current values of perhaps just twice the fuse value, it'll take a long time to operate.  
So remember the power of it is available to cause a temperature rise, there's a difference between the input power to the fuse as described by the I squared R of the resistance of the fuse.  
And the power that's being dissipated into the environment to the ampere fuse.  
And of course, the cable connecting the fuse.  
So fuses have an inverse pre-arcing current characteristic.  
If a current is above a maximum at which the equilibrium is achieved.  
Once the elements of a fuse and a conventional fuse have many elements once each element starts to melt the current flows in the liquid metal.  
Vaporisation of this liquid metal causes its resistance to increase and therefore the power going into a fuse increasing.  
So effectively, as resistance increases...  
I squared R increases.  
So remember pie equals I squared R.  
At that point, the metal in the fuse has melted, at this point the gap breaks down and you begin to get the arcing period.  
Generally, the duration of the transition between melting and arcing is very short.  
So the melting times on high occurrence can be very short and then the arcing process.  
And then the arc will continue generally until you get a current zero, when we get a current zero, the arc will be broken.  
The next slide is showing the process of an arcing period under a condition of a high current.  
So the fault current is significantly above the fuse rating.  
If I look at the perhaps there's an 80Amp fuse with maybe 400Amps that are flowing through the fuse.  
So effectively, when the arc is initiated there's a rapid increase in the voltage across for fuse element.  
And this can force a premature current zero.  
So if you look at the current characters, you can see that it's literally stopped the fuse early, stopped the current carrying.  
And the fuse has been designed to ensure the arc does not restrike.  
So they're carefully designed so that the arcing process begins in multiple points along the let's call it a fuse wire and then it does not restrike the arc.  
Fuses can operate very quickly, that diagram is showing a fuse operating in five milliseconds, so a quarter of the cycle.  
And it can cut off a fault current long before it reaches its first peak.  
So when you look at the diagram there, you can see that the fault current has been stopped at perhaps a third of its peak value and effectively the energy that's been let through into the equipment you're protecting is very small.  
In that diagram, the dotted line is, of course, the perspective fault currents.  
So this assumes the fuse didn't operate and that's the current that would've been passed through.  
If a fuse did not operate, ie.  
it would've been replaced, it wasn't a correctly graded fuse then of course that value of current would flow into the equipment you're protecting and that may result in the failure of the equipment you're protecting.  
In this case, the fuse operated correctly, it chopped the current at a lower value and it only let through a very small amount of energy into the cable of a transformer you're protecting.  
Again, following this process, if we look at the upper diagram this is showing the current.  
Then we have the pre-arcing period A, the arcing period.  
During the pre-arcing period the fuse affect the the silver in the fuse is beginning to melt and then once you get to the end of a pre-arcing period the melting process have continued is now effectively broken, an arc has now been established.  
So B is describing the arcing period.  
When you look at the lower diagram, you're seeing the voltage across the fuse.  
So of course, before the fuse starts to see the fault current, the voltage across the fuse itself is very small.  
Once the pre-arcing period, the fuse begins to melt and the voltage begins to slightly increase.  
So of course, we're putting there more heat into the fuse.  
At this point, when you get to the transition between the pre-arcing and the arcing period.  
Suddenly the fuse has got an arc across it, you're getting really a very high over voltage across the fuse.  
So you're seeing this fuse voltage is perhaps doubling a voltage across a fuse.  
Once the arc is finished at the end of time B and effective if this point the arc has gone out then of course, the voltage across the fuse is a voltage on one side.  
On the other side of the fuse, on the load side of the fuse the power has been disconnected.  
So what you're seeing there at the second stage of the third stage of our voltage signal you're seeing the Effective of a source emf.  
The next stage is showing the issue of the energy that's let through.  
And the energy let through by a fuse is referred to as I squared T.  
So of course, if you double the current, you quadruple the amount of energy let through if a fuse, of course, at the same time.  
Of course, as you increase the current in a fuse then the operating time significantly reduces.  
So when we look at that figure, we can see we've got a very high current and in this case the pre-arcing time is very short and then the cut-off current is reached just maybe one or two milliseconds after the fault occurs.  
At that point we enter the arching period, at this point, the current flowing through the fuse begins to reduce.  
And then finally at the time equal to the pre-arcing time plus the arcing time the fuse has extinguished the arc.  
The fuse has stopped the flow of current.  
And you can see that the energy we've let through into the equipment we're protecting, is very small.  
So when the current is high a fuse can cut-off in perhaps a quarter of a cycle.  
It's interesting, later on in this course we'll talk about protection, relays and circuit breakers.  
Generally, a protection relays and a circuit breaker will clear a fault in several cycles or perhaps, ten's of cycles.  
But in the case of a fuse, when there's high fault current the fuse operates in a fraction of a cycle.  
So when you compare the energy let through by a circuit breaker and the energy let through by a fuse under the case is a very high fault currents, then the energy let through by a circuit breaker is huge compared to the energy let through by a fuse.  
So in many ways, a fuse seems better than a protection relay and a circuit breaker.  
But later on of course, we'll begin to understand some of the limitations of using fuses.  
The next part is now gonna discuss, how fuses are applied to an electrical system.  
So fuses can be applied to two types of circuits.  
So circuits where the load is not very significantly above a normal value.  
In fact, those can be used for overload protection because if you know that your load current is always your normal load current is always a particular value.  
And then in the event of having an overload condition the fuse is capable of operating.  
But often you have situations where the load can vary considerably especially industrial loads.  
When you think about an industrial factor and you first energise a factor and energise an industrial process there's a very high value of current.  
So these fuses are an industrial process, commercial buildings are really there to provide short circuit protection.  
They're there to detect a fault and they're there to clear a fault and prevent damage to the equipment being protected.  
The selection of a fuse depends of course, on the maximum fault kVA of a circuit to be protected.  
It also depends on the voltages of a circuit.  
So if we think about that, maximum fault kVA is it a 100 kVA system is it a 1,000 kVA system?  
What is the fault level of the circuit being protected?  
It depends of course, on the voltage of a circuit is it a low voltage network operating at say 400 volts 690 volts?  
Or is it a high voltage network operating at 3.3 kilovolts or 11 kilovolts?  
It of course, also depends on full load current of the circuit.  
So of course, when we think about fuses we have to think about the current we're passing through the fuse under normal conditions.  
So if maximum load current is 100Amps and there is no inrush current as we first switch on the system we could perhaps use a 125Amp fuse to protect the 100Amp system.  
It's all about the degree of the overcurrent protection you required.  
Of course, if you used a 200Amp fuse to protect the network, whether the maximum load current was 100Amp it would mean that you would need effectively 300Amps before the fuse would operate.  
And at 300Amps the fuse would take a very long time to operate.  
So of course, you may discover there's inadequate protection.  
So again, when you're thinking about fuse you have to consider the level of all the current that must be carried for short time without blowing during the start-up perhaps to an industrial process.  
If you think about a motor when you first switch on a motor, there's a lot of energy enters the motor to start the motor to get the motor turning.  
And at that point we do not want the protection to operate protection is there to detect a fault.  
When you're using fuses as well, you must consider that the fuses need to grade with other protection devices.  
So perhaps a 400Amp fuse might need to grade with 100Amp fuses.  
And of course, a relay will need to grade with the fuses.  
So you have to look at how all these processes are working together.  
There are few rules of thumb, so these are like sort of accepted view points.  
So if you're protecting transformers, fluorescent lighting circuits when you first switch on a transformer, fluorescent lighting circuits and these are really low voltage equipment.  
Then you get a transient switching surge and what you will do is normally pick a fuse that's in a next highest rating above the full load current.  
So if your full load current was 150Amps you'd probably pick a 200Amp fuse.  
If you're protecting a circuit which its capacitors you'd use a fuse rating of greater than 125% of the full load rating.  
So if you've got a capacitive load use a fuse greater than 125% of its maximum load rating.  
And what you're doing is you're allowing this extra heating effect during the first energisation of a capacitator.  
'Cause when you first turn on a capacitor there's an inrush current.  
Motors are perhaps the most difficult problems.  
So if you're starting a motor directly from the AC mains, there's a starting current surge that normally lasts for perhaps tens of seconds perhaps, in this example 20 seconds.  
If you've got a direct online induction motor that starting current can be several times of full load current.  
If you're starting from an auto-transformer to start the motor, it will be perhaps three times the full load current.  
If it's a variable speed drive where the a soft start facility of course, the inrush current, starting current is significantly lower.  
So therefore it becomes less important.  
But in the case of a direct connection of induction motor onto a 400 volts supply, you must ensure you could cope with several times of full load current for perhaps 20 seconds.  
If you need all the load protection you probably put a setting of perhaps twice the maximum load current.  
In summary, fuses are simple, fuses are inexpensive and they're reliable.  
And of course, fuses have been used for a very long time.  
They provide very fast clearance of high current volts.  
There are limitations of course, fuses can only detect faults which are associated with high values of current.  
A fuse has an operating characteristic that cannot be adjusted or set.  
Of course, you can change a fuse and put a higher rating or a lower rating fuses but you need to physically change it.  
Once a fuse operates, it needs to be replaced.  
And generally, fuses can only be used on low or medium voltage, so perhaps very commonly used on low voltage networks, so 400 volt networks or less than 1,000 volt networks.  
And they will then be used on less important low power medium voltage circuits, so perhaps 3.3 kilovolts systems in rural areas, 6.6 even 11 kilovolts systems in rural areas.  
But generally, there are less important power networks of the medium voltage level.  
I hope you enjoyed the talk about fuses and we will move in the next talk towards all the current protection using relays.  
Thank you.  
  
  
# 1.4 Recommended - Current and Voltage Transformers  
--LECTURER:  
Hello, I'm Peter Crossley I'm professor of power systems at the University of Manchester.  
My talk today is about power systems protection.  
And starting off as an introduction, with voltage and current transformers.  
Voltage and current transformers are there to protect the...  
protection relays and the measuring equipment .  
So when you consider a primary power system.  
It is operating at hundreds of thousands of volts or tens of thousands of volts and it is operating at current levels from hundreds of amps to thousands of amps.  
When you look at a protection relay, it's constructed using intricate fragile electro-mechanical movements, many ways similar to a clock or it operates using sensitive microprocessor based systems.  
Obviously if we put into those relays, hundreds of amps or thousands of amps they would be damaged.  
So what we have is CTs and VTs which are an essential part of the protection system.  
They're designed to reduce both the primary current and voltage to a low level that's suitable as the input relay.  
So we take perhaps a nominal current of 2,000 amps.  
We reduce it to a secondary current of 1 amp and we apply the 1 amp to the protection relay.  
Protection relays are of course operate under fault conditions.  
So, during a fault, the 2,000 amps might increase to 50,000 amps.  
So in the case of 50,000 amps, we got 25 times the nominal current.  
So, we got 25 amps flowing into the relay.  
So, CTs and VTs are an essential part of a protection system.  
In fact possibly the most essential part of a protection system.  
So we must be correctly specified to satisfy the operating requirements of a relay.  
And correct connection of CTs and VTs is essential to the performance of the protection.  
So, a voltage transducer converts for primary voltage being measured from some Kilovolts perhaps tens of Kilovolts to hundreds of Kilovolts or even to a thousand Kilovolts and converts it to a secondary voltage in volts.  
In the United Kingdom we always use 110V on the secondary of the VT ratio.  
So VT ratio, so the voltage transducer ratio is the nominal primary voltage expressed as a line to line RMS voltage.  
So, for example 132kV or 400kV or 11Kv and is then converted to a secondary RMS voltage which is 110 volts between the phases.  
So its a line voltage and it's the...it's 100 volts in the UK.  
Most of the world uses 110 volts as a secondary voltage.  
A small number of countries including The United States operate at 125 volts.  
These voltage transformers can either be capacitive voltage transducers or can be wound type voltage transducers.  
Generally wound type voltage transducers are used at sub-transmission distribution voltage levels and at transmission voltage levels.  
So perhaps 400kV we generally use a capacitor divider.  
With a wound voltage transformer on the secondary.  
So the capacitor divider reduces voltage from 400kV to 11kV.  
And then a transformer reduces it from 11kV to 110V.  
So a current transducer converts for primary current to be measured from Kilo Amps to a secondary current in amps.  
And normally, the...so if you consider national grid, they generally use 2,000A CTs on the 400kV system.  
And 1,200A CTs on the 275kV system.  
So those are the primary current they're the nominal primary current.  
It really defines the maximum load current seen by the relay.  
This nominal primary currents are then converted down to 1A or 5A.  
So effectively we have for example 2,000 to 1CTs, so it's taking 2,000 amps on the primary and it's converting it to one amp on the secondary.  
Alternatively under fault conditions, perhaps the current is 10,000A on the primary which will then convert down to 5A on the secondary.  
Or if it was 20,000A it would convert to 10A on the secondary.  
We also have current which are rated with a 5A secondary.  
So these basically for example a 600 to 5A CT.  
A 600A on the primary and 5A on the secondary.  
When you look at these CT ratios, generally the 1A secondary CTs are used at the higher voltages and 5A secondary CTs are used at the sub-transmission distribution voltages.  
Although it isn't always true and occasionally we have 5A CTs used on 400kV systems in the UK.  
The example quoted on the slide is a 5A CT so it's a 5A on the secondary but nominal current on the primary is 800A.  
So during fault conditions, if a fault current was 8,000A, there would be 50A on the primary...  
on the secondary.  
VTs operate using electromagnetic or capacitive transformation principles.  
In other words, electromagnetic is effectively a transformer.  
And the capacitive technique is the capacitor divider, is generally referred to as a capacitor voltage transformer or a capacitor voltage transducer.  
We now almost...we now gonna concentrate on current transformers which is one of the most critical aspects of a protection system.  
And we gonna start by saying we have two basic groups of current transformers.  
We have measurement current transformers which is designed to operate on very limited current range.  
So, if you have a current transformer which is capable of working up to 1,000A on the primary, it is really designed to only work up to a maximum current of perhaps 1,200A on the primary.  
And it is not capable of going beyond that.  
So, it works always around the nominal current.  
It is really used for measurement purposes.  
So, it's measuring the normal current flowing in the line.  
We also have something called protection current transformers.  
These are what creates the current that goes into a protection relay.  
These have to operate over a wide range of currents.  
So, for example under normal conditions, they, for example, a 2,000A to 1A CT measure 2,000A on the primary 1A on the secondary.  
Under fault conditions that might increase to 70,000A and we might get 35A on the secondary.  
So it's working over a huge range of current conditions.  
This means that the measurement CTs and protection CTs are designed differently.  
They use different material and they are designed for different operation purposes.  
So, we're really gonna concentrate on protection current transformers which are what powers of protection relay or what provides the input current signals for the protection relays.  
The diagram shows a picture of two types of CT.  
One is referred to as a bar primary CT.  
This is probably the most common type of CT where effectively we've a single winding on the primary a multiple turns on the secondary.  
So, for example we got one turn on the primary and perhaps 600 turns on the secondary.  
Then we've wound primary where we put multiple turns on the primary.  
And obviously a large number of turns on the secondary.  
So perhaps we might have five turns on the primary and perhaps we've 1,000 turns on the secondary.  
So in terms of its turns ratio, five on the primary, 1,000 on the secondary is equivalent to effectively 1:200 ratio.  
This example shows a picture of a current transformer in which the primary and secondary windings are encased in epoxy resin.  
This is typically used in applications such as 11kV switchboards.  
So, you can see there the effective of a bar primary is designed to go through the aperture at the centre of the CT.  
Then you have an iron core.  
And then around iron core is of course many, many secondary turns.  
And then you have a resin casing to protect it and to stop damage or to stop flashovers.  
These pictures are showing examples of current transformers being used at very high voltages in outdoor applications.  
In the United Kingdom most of our transmission substations are effectively outdoor substations.  
So we have large numbers of these CTs which were mounted at the top of a large porcelain, ceramic Insulator.  
so part of an insulating system.  
So these current transformers basically provide the insulation, as well as convert the high currents on the primary into a low current on the secondary.  
And of course this current transformers are designed to have a very long operating life.  
So perhaps they will successfully work for 50, 60, 70 years.  
Experience with conventional current transformers, has been extremely successful.  
They have been used for nearly 100 years and have proved to be have an extremely long life.  
This is showing the differences between a protection CT characteristic and a measurement CT characteristic.  
It is showing this BH curve.  
So B is the flux density within the core, H is the magnetising current multiplied by a number of turns.  
You could have drawn that slightly differently using the secondary voltage from the CT versus the excitation current.  
I will explain later the excitation current is really a problem because what it's doing is it's removing current from effectively, the primary current referred to the secondary and is causing errors.  
When we look at measurement CT it has a different characteristic to the protection CT.  
You require very good accuracy in the measurement CT up to approximately 120% of rated current.  
So you really need the accuracy from 0% to 120%.  
So if you've got 100A measurement CT you want it work successfully we're measuring steady state sinusoidal current from 0A RMS up to maximum of 120 A RMS.  
These require a very low saturation level.  
So they are designed to have this characteristic where we take very little excitation current.  
And actually then we go, once we get beyond 120% of the current, their operating level, they begin to go into deep saturation.  
They use a nickel iron alloy core which has a very low exciting current as shown in that diagram.  
You can see that the vertical part of the measuring CT.  
The H value which is effectively excitation current is very, very small.  
The knee point voltage of this low flux density levels is about 0.7 teslas.  
When we look at protection CTs and this talk is really gonna now concentrate on protections CTs.  
The actual absolute accuracy is less important, what matters is its behaviour under very high fault currents and avoiding the problems of deep saturation in the core.  
In this case we must operate at many times their rated current, typically 20 times or 30 times their rated current.  
And these cores are carefully designed using cold rolled grain oriented silicon steel of C.R.O.S.S.  
It has a high saturation flux density, this diagram shows 1.6 teslas.  
That's actually a value for very traditional CT.  
Now you will probably be using better materials which is reaching 1.8 teslas in its flux density.  
But you must remember that a current transformer will probably operate successfully for perhaps 60 to even 70 years.  
So consequently there are many old current transformers in the system.  
This slide is showing the calculation for a knee point voltage.  
And we've derived an equation which is EK equals 4.44 times Bk times A times f times N.  
We will do a whiteboard exercise to derive that equation, but basically it comes from the classical Faraday equation as EMF equals minus D phi by Dt.  
So what we do we take the flux value of flux so we take flux peak sign omega T we differentiate it to get omega flux peak cos omega T.  
Then we realise that Ek in that diagram is the secondary induced voltage is an rms value.  
So we then divide that calculation by the square root of two to create rms.  
We realise that the flux peak is equal to the flux density peak multiplied by the cross sectional area of the core.  
F is of course the frequency so in the United Kingdom 50Hz.  
Actually interestingly in the United Kingdom of 50 hertz systems with a slightly larger CTs then we would use on 60 hertz by the American system.  
And then of course, N is the number of secondary turns.  
So that is the equation.  
If we now look at an example, we take a CT with a ratio of 2,000 to five with a cold road oriented silicon steel core, with a flux density at 1.6 teslas.  
So the core cross sectional area is 20 centimetres squared.  
The maximum current is 40,000 amps.  
So what I'm going to ask the question is what is the maximum secondary burden permissible if core saturation is to be avoided?  
So if we got a maximum flux density of 1.6 teslas, we've got a cross sectional area 20 times 10 to the minus four metres squared.  
We got a turns ratio of 2,000 to five, effectively the 400 to one.  
We got a frequency of 50 hertz.  
If we put all those values into the equation, we get an answer of the knee point voltage is 284 volts.  
So the maximum secondary current is of course, 40,000 amps divided by the 2,000 to five ratio of the CT which gives an answer of 100A.  
So we got 100A coming out of the CT and the steady state sinusoidal conditions where there is 40,000A in the primary.  
So to get a voltage of 284V, the burden resistor could be 2.84 ohms.  
So 2.8 ohms.  
You will learn later that this is a simplification and many of the problems with CTs are caused by something called DC offset.  
I will talk about that later, but when we've got a value there of 2.8 ohms in practise we would want a value of significantly even less than one ohm to ensure that it works under DC offset.  
I will talk in detail about that in a later slide.  
When you look at the transformer polarity, this is showing a diagram which is showing that the primary current is flowing from p1 to p2.  
The CT orientation is effectively means that the current flows out of terminal S1 and returns to terminal S2.  
So the relay is connected between S1 and S2, the polarity becomes extremely important because most protection systems compare the current to the voltage or compare the current in one location to the current in a different location.  
So if you connect the current transformer in the wrong direction.  
So with a wrong orientation, or the wrong polarity, you'll get the wrong operating time.  
Of my time working in protection, I have seen serious maloperations caused by incorrectly commissioned current transformers where the orientation has been in the wrong way round.  
In fact, I know of one example where the CT which was driving a distance relay for transmission feeder protection was actually in the wrong direction so effectively the relay was looking into the busbar.  
Rather than looking into the transmission line.  
So this is showing the basic theory of a CT.  
We have a current flowing of Ip, this creates a current of Is, so Is is the secondary current.  
So Is is equal to Ip divided by the turns ratio of the transformer divided by N in this case where N is the number of secondary terms.  
So the primary current is equal to N times the secondary current, or more important the secondary current is Ip.  
Divided by N.  
Again this is showing the structure as we connect a CT to a relay.  
In this diagram I've assumed the relay wiring, the CT resistance are resistive.  
And this is then connected to a burden ZB.  
As shown in that diagram, ZB is the lead resistance and the relay impedance.  
In the case of a modern numerical relay, the relay impedance will be a pure resistor.  
In the case of elctromechanical relay, the burden will be resistive and inductive.  
So it's an inductive burden...  
is an impedance burden.  
ES equals IS times ZB, so in that diagram you can see that IS is IP divided by the turns ratio.  
So ES equals IsZb, which is equal to EK which is the voltage at the effectively the fictional.  
So the internal turns ratio of an ideal CT, and then we've got RCT, which refers to the winding resistance.  
This is because a CT, the wire is made using copper, and copper of course is resistive.  
So what we've got that ES equals EK minus IS times the wiring resistance of the CT.  
And now we're gonna define what I mean by knee point.  
Knee point is critically important, because as you go beyond the knee point, you begin to get saturation effects.  
Our definition of knee point is, that a 10% increase in voltage above the knee point voltage value, requires more than a 50% increase in current.  
So basically 10% increase in voltage, creates a 50% increase in current.  
This is where core of the current transformer, is beginning to saturate.  
This slide is showing the equivalent circuit of a current transformer.  
So on the far left hand side, you can see that you have a primary current passing through the primary conductor.  
Then you have this ideal representation, remember this is only an equivalent circuit.  
So you then have an ideal current transformer which is producing a current on the secondary coming out of S1, which is the primary current divided by the turns ratio.  
Then because remember this is an equivalent circuit, we then have the magnetising branch of the CT.  
The magnetising branch is describing the excitation current, the current taken to excite the core.  
So i.e.  
the excitation current is of course current being taken out of the CT circuit.  
So the actual current leaving the current transformer IS, is equal to the primary current divided by the turns ratio minus the excitation current.  
To reduce the excitation current, we should use of course a big CT, so that the current transformer does not saturate, but of course large CT's cost more money and require more physical space.  
So you'll learn later that the size of a CT is really a compromise between its electrical performance and its physical dimensions and weight.  
The secondary current IS , which is equal to IP divided by N minus IE, then passes through the CT wiring circuit plus the leads, 'cause of course the actual relay described as ZB, is remote from the CT.  
So ZB is the relay, and what we are interested in is the secondary terminal voltage at that point.  
So within what is referred to in that diagram as ZCT, we have the CT impedance and we also have the lead resistance.  
This diagram is getting you to think a little bit of some of the issues about the CT.  
So for example we have a primary current of 100 amps.  
We have a CT ratio of 100 to one.  
So the secondary current is one amp.  
In the case where we connect that CT to one ohm resistor, we have a voltage across for one ohm resistor of just one volt.  
So the expectations are that that would be low down on the BH curves, so on the excitation curve of the CT as shown in the diagram.  
When we have a load of 10 ohms, of course now that the voltage required drive a current through the 10 ohm load, is equal to 10 volts.  
Because it's one amp times 10 ohm.  
If you had 100 ohm load, then you need a voltage to drive the current of one amp through the CT of 100 volts.  
And of course by now, with 100 ohm load in this very idealistic diagram, we're beginning to get saturation, the excitations current is going higher.  
So for example, if instead of 100 ohms it was 120 ohms in that diagram, you can see that the excitation current becomes very significant and basically the CT begins to saturate.  
Interestingly if of course we were to connect 1,000 ohms to it, we would require an EMF of 1,000 volts to drive the current.  
If for some reason the secondary of a CT becomes open circuited, so say for some reason there is a poor connection to the CT, it's got an open circuit, you get a huge voltage which is basically above the knee point voltage of the CT.  
And that of course could cause damage or could be fatal to a human.  
So you have to be very, very careful, that CT's are connected to a low impedance burden.  
This diagram is showing the impact of current transformer saturation.  
So we have a primary current, of course now this is under steady state sinusoidal conditions.  
This is assuming you are on the steady state condition, a fault has occurred, you've waited until the transients have gone away, and this is the steady state condition.  
And you can see that the flux is now deeply saturated as it's reached its limit.  
And at that point, the secondary current is distorted because you must remember that EMF equals minus D phi by Dt So consequently once a flux becomes affected to be DC, there is no EMF at the output of the CT, so there is no current.  
So the secondary current is severely distorted.  
This problem is a serious problem which we'll look at in other parts of the lectures.  
'Cause in the previous parts of the course, you began to study about the impact of faults on power networks.  
You learnt about three phase faults and phase to phase faults and single phase to ground faults.  
And also you began to learn about the point on wave of a fault.  
So if a fault occurs at 90 degrees, it's a voltage maximum.  
And the circuit is an inductive circuit.  
And actually the current is correct and the secondary current will still look sinusoid.  
But imagine what happens if a fault occurs near a voltage minimum on an inductive system.  
Then what happens you get a DC offset.  
And a DC offset is now causing a major problem to the behaviour of a CT.  
So the primary current has got this DC level.  
Normally when we think about a transmission system, we generally perceive that the X upon R ratio will be 20, 30 or 40.  
And that way the DC offset can last if the X upon R ratio is 40, the DC ratio could take perhaps 100 milliseconds before it decays away.  
So with the CT, we are trying to pass a DC through the CT for a time period of perhaps 100 milliseconds.  
This is causing us a major problem because the CT will now go into deep saturation.  
To avoid saturation, this will be explained using white board activities during tutorials during discussions with the tutors.  
But during these conditions where you've got a DC offset caused by a fault which is occurring at a voltage minimum if it's a phase to ground fault.  
Then what we should do is we should overdimension the CT's.  
But if we calculat that under steady state conditions, we'll require the CT with a knee point of 200 volts.  
If this is then used on a transmission system, which has got an X upon R ratio of 40, we should use a CT with voltage rating of 200 volts multiplied 40 plus one for the steady state, so you get this X upon R plus one, multiplied by the steady-state knee point voltage.  
So in the case of that example, if the steady-state knee point voltage was 200V, we would require 41×200V so we'd require 8.2kV.  
We've got very huge CTs.  
Of course we can't afford to use huge CTs.  
So it's a compromise.  
So with protection relays are designed to cope with CT saturation.  
And we design systems where during the switching on process when the fault first occurs, the protection relay can cope with CT saturation.  
CT saturation is less of a problem on distribution network so especially on utility distribution networks.  
Because generally on a distribution network, the X/R ratio is probably five and consequently if you have a CT with a knee point of 200V and a steady-state calculated conditions.  
We'd need a value of (5+1)×200 so 6×200.  
So we need a knee point of 1,200V.  
That's still a high knee point for a distribution CT.  
The really complex problem is if we have a fault on a offshore oil platform where the X/R ratio is extremely high because there's very little resistance in the circuit.  
All the generators and the motors and the pumps, all physically close together.  
So there's a lot of inductance in the system, all the transformers are close together.  
So when we need to use start using all the dimension CTs, this will be discussed in more detail as we move into the more detailed part of this course.  
When we look at CTs from a protection's perspective, we have something referred to as 5PCTs, 10PCTs.  
So for a 5PCT, the accuracy class 5P converts to a limits of error so under rated current.  
So for example, it's a 600A to 1A CT, a 5PCT will have an error of 1% at 600A.  
But then we have something called the fault current limits so this is where we define that the 5% distortion comes from.  
So if we define a CT with an accuracy fault so with a fault current limit of 20 times, a 5PCT as a 5% error, at 20 times rated current.  
If it's an accuracy limit of 30 times, it will be a 5% error of 30 times of rated current.  
If we have a 10PCT, this is an error under rated current condition.  
So for examples at 5A CT would have an error of 3% at the 5A secondary current.  
And that the fault current limit would have an error of 10%.  
So at 20 times rated current or 30 times rated current, depending on your specification will be a 10% error.  
So when we talk about CTs, we talk about its rated Volt Amperes.  
We talk about the class of the CT whether it's 5P or 10P.  
There's also something called Class X which we will discuss in the tutorials.  
And when we talk about the accuracy limit factor, that's the maximum current which the accuracy level is maintained.  
So for example if the value of burden...  
The value of burden really defines the size of its CT so for example you can have a burden of 2.5VA, 10VA, 30VA.  
And this of course is defining the physical size of the CT.  
Then we have the 5P, the 10P and then we have the accuracy limit on fault current.  
The rated burden in ohms is defined as the rated VA divided by the secondary current squared.  
When we look at a Class P, this protection CTs, as I mentioned rated burden a Class 5P has got a 1% error of rated current, 5% error of the maximum fault current.  
It has a 10PCT, that's 3% error rated current and 10% error maximum fault current.  
Then we have to consider the accuracy limiting factor which in the example shown there, we've got 50VA CT, we've got a 10P class of CT, which means it's got a 10% error at the maximum fault current.  
The maximum fault current to maintain the 10% error is 20 times the nominal current.  
So to convert the Volt Amperes and the accuracy limit factor in useful Volts of a knee point, we take the voltage of a knee point is the volt amps times the accuracy limit factor divided by the nominal current and that converts to 300 divided by In.  
So the knee point voltage is 300 divided by the nominal current.  
So in the case of a 1A CT, it would be 300V where the nominal current is 1A.  
In the case of a 5A CT, it would be 60V.  
The rated burden is the value of a burden upon which the accuracy claims are based.  
We express it in Volt Amperes.  
We have some preferred values:  
2.5, 5, 7.5, 10, 15, 30 VA.  
The continuous rated current is what the CT will carry current continuously so without damage.  
Of course under fault conditions, fault currents are significantly higher and the CT can only operate for a short time with fault current.  
Short term rated current which is really about the fault current.  
It's usually specified for perhaps 0.5 a second or one second or a few seconds.  
As long as a fault current is maintained less than this few seconds, there are no harmful effects.  
Although when we define the short time rated current, we tend to specify it with the secondary shorted.  
To try and understand behaviour.  
As I mentioned earlier, the rated secondary currents on a CT on almost always 1A or 5A.  
Very occasionally, you will see current transformers with a 2A secondary.  
So when we're looking at the choice of the CT ratio, what we have to do, we have a primary rating.  
So you've got the normal current in the circuit and then you've got the thermal continuous rating must not be exceeded.  
So obviously we can't damage the current transformer.  
We have to ensure that it's capable of operating at the thermal limit.  
The secondary rating as I mentioned before, is normally 1A or 5A.  
The secondary wiring route length...  
If it's short, we can afford to use 5A CTs.  
If it's greater than 30m, we tend to use 1A CTs.  
So in this case, a CT with length greater than 30m, we will use a 1A CT at the secondary.  
The maximum ratio of the CT is normally 3000 / 1.  
When I look at national grid, their maximum ratio CTs they use on the 400kV system in the U.K.  
It's 2000 / 1.  
On the 275kV system, it's 1200 / 1.  
When you have a very large generator, you will sometimes use very large CTs and perhaps 3000 / 1 as a CT ratio.  
But sometimes, you'll use a main CT then with an interposing CT.  
With these large generators are a special cases.  
So this example, I quote an example we're using a 20A secondary CT so it's a 5000 / 20.  
And then it's got an interposing CT so a second level of CT that's going from 20A to 1A.  
This is a really a very special requirement for generators.  
Thank you very much that's the end of my talk on current transformers.  
We will be discussing current transformers through almost all parts of this course and during the exercises which we're going to continue with you.  
We'll begin to explain some of the difficulties in using CTs, the impact of X upon R ratios, the impact of a point on whether the fault on the DC offsets in the current or the exponential offsets in the current.  
So I hope you enjoyed this talk on current and voltage transformers.  
Thank you.  
  
  
# 2.1 Overcurrent Protection – Grading By Current & Time  
--LECTURER:  
So discrimination by time sees the highest current faults cleared in the longest time.  
And this is a great problem because if you have a fault located close to the source, the clearance time is long.  
If you discriminate by current, you require an appreciable impedance difference between the breakers.  
Therefore, what we tend to do is begin to discriminate by time and current.  
And in British practice, we tend to use relays which have these Inverse Definite Minimum Time operating characteristics, referred to as IDMT relays, and effectively the higher the current, the faster they operate.  
Most of this lecture will be about grading of IDMT relays.  
This is showing a very early IDMT relay, which actually has been manufactured in the UK many countries around the world for, I guess 80 years.  
These are classical electromechanical relays.  
When you look about relay, they have an operating solenoid, which creates a magnetic field in conjunction with the second coil perpendicular, and it basically moves the disc.  
This as I mentioned in the introduction is effectively a modified form of a classical electromechanical Ferraris disc watt-hour metre so as we pass the fault current through the coils, the disc turns and if you look at the mechanism you can see this as an actuating bar which moves across and then touches the contacts by touching the contacts, it activates the auxiliary reliever, small electromechanical relay which then closes the contacts.  
When you look at the process of that relay, it's got a spring, which is an opposing spring.  
Effectively a relay is really like a clock so you have jewelled movements to control it all.  
When you look at the settings you have something called a time multiplier setting.  
If you set the time multiplier setting to one, the particular relay would have the standard inverse operating time.  
If you set it to 0.1, it would operate in 10% of the standard operating time for particular value of current.  
You also have something called a plug multiplier, the word plug multiplier comes from the plug which you inserted in to this type of relay, and that really defines the number of turns you connect within the electromagnet.  
So as you connect more turns in the electromechanic magnet, you make the relay more sensitive, so you can produce a characteristic which is an inverse time characteristic, it has a time multiplier setting you can change and it has a plug setting you can change.  
So the relay operates from the current flowing through an operating coil exceeds a user-defined threshold for a time period specified by the user.  
In this particular type of relay, if the current is significantly above the user-defined setting, it has a very fast operating time.  
These are the mathematical equations we use to describe this.  
Of course, electromechanical relays were designed many, many, many decades before we ever introduced the equations.  
Actually, when I look at the equations, electromechanical overcurrent relays were designed in the 1920s, and these equations began to be used in the 1980s, when people began to replace electromechanical relays with modern numerical relays, and as soon as we designed the numerical relays obviously mathematical processing systems, we needed to have a mathematical equation.  
British practice, so British standard inverse, the standard inverse characteristic in accordance with the IAC characteristics has the operating time:  
t=0.4 divided by I raised to the power 0.02 minus 1, where I is a fault current expressed as a multiple of the setting current.  
All those equations assume a time multiplier setting of 1.  
If you have a time multiplier setting of 0.1 then you would multiply all the answers by 0.1 The very inverse characteristic has a mathematical equation of 13.5 divided by I 1.  
And then extremely inverse has a mathematical equation described as 80 divided by I squared minus one.  
I emphasise again that 'I' is the fault current expressed as a multiple of the setting current.  
What you must remember about those equations, those are mathematical equations which are trying to model characteristics, which were experimentally derived almost a hundred years ago, so we are producing a mathematical model to allow us to model the behaviour of a classical electromechanical standard inverse relay of an electromechanical very inverse or an extremely inverse relay in a numerical system.  
Let's look at some examples.  
I looked for an example of a standard inverse relay which has got this equation operating time equals 0.14 divided by the fault current divided by the setting, the setting current value, raised to the power 0.02 1, and this is then multiplied by the TMS.  
First question, of course, what is the primary fault current?  
This simple example, I have assumed we have a primary fault current of 3200 Amps and the current transformer ratio is 400:5.  
When you look at that, you can see that during a fault, you have a value of 40 Amps flowing because of course 3200 Amps is 8x400 Amps, so in fact the current value which is flowing is 8 times the nominal current value.  
The nominal current value is 400 Amps on the primary rate and 5 Amps on the second.  
So 3200 Amps on the primary is eight times nominal and this translates to 40 Amps on the secondary.  
Now if we set the relay with this setting current of twice nominal, so we set the relay to operate at 10 Amps on the secondary or 800 Amps on the primary, if fault current is 3200 Amps, we have a current value four times the setting value.  
So the fault current is four times the setting value, this will flow through the relay, When you look to the operating characteristics in the next slide, you will see that the standard inverse operating time is five seconds using that equation.  
So if we went to the equation and with your calculators, you said that 0.14 divided by 4 raised to the power 0.02 minus 1, and in this case if the TMS is 1, it gives an answer of five seconds.  
We can of course adjust the operating time by changing the time multiplier setting.  
And the time multiplier setting, the time multiplier setting of 0.2, the standard inverse operating time is one second, if we have a time multiplier setting of 0.1, the standard inverse operating time is 0.5 seconds.  
Of course, when you're doing your grading studies, you have to determine suitable values for the setting current and suitable values for the time multiplier setting.  
In British practice or IAC practice, we have standard inverse relays, we have very inverse relays, and we have extreme inverse relay, but the previous slide showed the mathematical equation.  
This is actually showing a picture showing the mathematical equation converted into a diagram, so we got a log, log scale, so the y-axis is showing the operating times and the x-axis is showing the current as a multiple of setting, so when you look at those equations, if for example the current was ten times the extremely inverse relay operates in 0.6 of a second, the very inverse relay operates in 1.3 seconds.  
Remember these are logarithmic scales, and the standard inverse relay operates in 2.8 seconds.  
Of course these times are then adjusted by the TMS.  
So these operating characteristics need to be selected based on the need to coordinate with other devices on the network.  
So remember that, that furthest down stream relay will probably need coordinate with fuses, or circuit breakers in the low voltage network.  
The upstream relay will need to coordinate with the downstream relay.  
The upstream of the upstream relay will need to coordinate with the upstream relay.  
So you've got this process always of coordinating with all of the other devices in the network.  
And of course what we are trying to determine is the tripping time required for high and low current faults and we are looking at how the complete network goes together.  
Important issues are related to the maximum fault current and the maximum load current.  
Of course if the, load currents are low and the fault currents are high it's an easy protection problem.  
But of course we also have the inrush currents of transformers and motors, and we must ensure that protection remain stable when you first switch on an industrial complex, or switch on a transformer, switch on a motor.  
And of course the other factors, what is the minimum fault current?  
When we say minimum fault current, we tend to mean, a solid fault, we tend not to think about resistive faults at this point Although later, we'll have look at some of the challenges created by resistive faults on networks.  
I did some calculations here, so I went through an example, I wanted to calculate the standard inverse, very inverse and extremely inverse, the operating time if the setting current was 150% of 5 amps, the time multiplier setting was one, or perhaps .1, obviously in a real system, those two values have to be calculated based on grading studies.  
Obviously just to get you to understand how to use the mathematical equations and how to understand how to use the curves.  
So in many senses I want you to take this table and I wanna make sure that you can create the same values.  
We've got a current-transformer ratio of 600 to five, So of course if we have 600 amps on the primary, we would have 5 amps on the secondary.  
If we now complete our table for different values of fault current, I've assumed the fault current is 1800 Amps, is 3600 Amps, is 7200 Amps and is 14400 Amps.  
Of course 1800 Amps is three times the nominal current value, where 3600 Amps is six times the nominal current value, 7200 Amps is of course 12 times nominal and 14400 is 24 times I nominal.  
So we were doubling the fault current.  
The setting current was set at 150% of the nominal current.  
So in fact the fault current as a multiple of setting increases from twice setting to four times setting to eight times I setting to 16 times I setting.  
When we put those values on the curve of the standard inverse curve, and of course when we're looking at a curve, it's a logarithmic scale curve and we are not getting the exact values, but it's approximately correct that, for a value of twice I setting and a TMS of one, we get 11 seconds, for a value of four times I setting and TMS of one we get five seconds, the value of eight times I setting and TMS of one we get 2.9 seconds, and for value 16 times I setting we get an operating time of 2.3 seconds.  
Just now playing a little bit.  
So what I'm gonna do now is put the values into the mathematical equation for the standard inverse relay.  
This is calculated now at 10 seconds, five seconds, 3.3 seconds and 2.4 seconds.  
Just for illustrative purposes, I've then put a TMS of 0.1 so of course my values become one second, 0.5 seconds, .33 seconds and 0.24 seconds.  
These are the standard inverse values.  
So the standard inverse operating times.  
If we now take the very inverse equation, we get values of 13.5, 4.5, 1.9 and 0.9 and of course, you could repeat it and do the very inverse curves, look at the curves and see what values you obtained.  
And then if we put a TMS at 0.1, 1.35, 0.45, 0.19, and 0.09.  
When you move to the extremely inverse equation, if we put a TMS of one, we get an operating time of 26.6, 5.3, 1.3 and 0.32.  
So when you look at the extreme inverse very very fast on high fault currents and very slow on low faults currents.  
Of course we could again play with the TMS, so we just written the value for TMS of, a time multiplier setting of 0.1, we get a value of 2.7 seconds, 0.53, 0.13 and 0.03.  
I want you to look at those numbers and I want you to think, which is the best relay?  
Which is the relay we should use?  
And I will be honest, you can't answer it, it's an impossibility, 'cause it depends on what you're grading with, It depends on the performance of the other protection systems.  
So as we move through this course, we'll generally look at how we perform a grading study.  
So whether you decide a very inverse, extremely inverse, or standard inverse.  
How do you decide on the settings?  
The current settings.  
How do you decide on the time multiplier settings?  
In addition to inverse time overcurrent relays, we have definite time overcurrent relays.  
These have basically an operating time which, when the current value is above a setting value, they operate in a fixed time.  
So for example, if I look at that case, this is a very simple relay I've just borrowed some examples, so D8 is an operating time of eight seconds, multiplied by the TMS value, D4 has an operating time of four seconds multiplied by the TMS value, and D2 has an operating time of two seconds multiplied by the TMS value.  
What that means is, and when you look on the x-axis, you can see this is a current as multiple of setting.  
So if your fault current is greater than your setting current and if you have a D8 element, it would operate in 8 seconds multiplied by TMS of, perhaps for example, you set a TMS of 0.1 you get an operating time of .8 of a second.  
In the United Kingdom, definite time relays are often used to reduce the operating times of inverse time relays when the fault current is low.  
So perhaps if your inverse time relay is giving an operating time of tens of seconds, you could use it in conjunction of the definite time relay, to bring the time down to perhaps one second.  
So again, they're used in conjunction with IDMT relays and subsequent slides will illustrate this process.  
So for example you can take a definite time relay you could set it, but it always operates in one second, if fault current is great than I setting, where the setting value's probably in that case quite a low value, perhaps it's been set to one and half, or twice the maximum load current.  
In addition to the various inverse operating characteristics, or definite time, inverse times, we also have instantaneous operating characteristics.  
An instantaneous relay operates as quickly as possible when the fault current exceeds a fixed setting.  
So if a fault current is very high, we set the relay to operate as fast as it possibly can.  
So for example an instantaneous relay can be set to operate instantaneously when the fault current is great than I setting.  
And normally we would expect the setting value would be high to reduce the risk of a grading problem.  
When we say instantaneous from the context of overcurrent protection, we tend to expect the relay to operate in about 100 milliseconds.  
This line now is showing this combination, so in the centre of the slide we're seeing a standard inverse, IDMT characteristic.  
When the fault current is very high, so is greater than 20 times, the relay operates as in instantaneous element.  
In this case I've shown it with an operating time of 200 milliseconds, perhaps 100 milliseconds for relay and 100 milliseconds for the circuit breaker.  
So we're seeing this behaviour.  
So in this case, we got an operating time at the instantaneous of 200 milliseconds.  
The inverse time is going from an operating time of 700 milliseconds at 20, well just less than 20 times second, 20 times settings to a current of three seconds.  
Sorry, to an operating time of three seconds when the current is 2.5 times the setting.  
When we're below 2.5 times setting, we move to a definite time.  
And the definite time relay operates in three seconds when the current is between, it's effectively greater than the setting and when the current is less than three, 2.5 times the setting.  
So we're using this combination of characteristics.  
So we've got definite time of the low currents, inverse time, mid-range currents and we've got instantaneous and very high current values.  
When we're looking at overcurrent protection, the issue is about grading.  
And we discuss things called the relay to relay grading margins.  
This is really referring to the difference in the required operating time of the upstream and the downstream relays when a short circuit fault is located just beyond the downstream relay and your source capacity of your network of a point of a fault is operating at a maximum level.  
What that means is that the downstream relay is seen the highest possible fault current and the downstream relay has its fastest operating time.  
What we're trying to ensure is that the upstream relay does not operate if the fault is downstream, of the downstream relay.  
The reason for that is if the upstream relay operated, we disconnect large numbers of customers on feeders which are not faulted.  
Ideally, the downstream relay should clear a downstream fault.  
But if for some reason the downstream relay is not capable of clearing the downstream fault, then the upstream relay provides backup.  
We have this equation for grading margin, this is the traditional equation we use.  
So the grading margin between the two relays at this maximum value of current for the downstream relay is twice the relative timing error in the relays which in this case I've given an example of +5% and -5%.  
My concern is that the downstream relay goes 5% slow and the upstream relay goes 5% fast which is why we got twice and we got this two times this 5% error.  
Then we've also added to that the relative timing error due to the effect of the CT.  
This is related to saturation of the CT and it's causing the current, it's causing operating time to be slow.  
This is because the current coming out of the CT is less than you expect.  
So we were assuming the downstream relay is saturated and is producing a current value, that's affecting the operating time by 10%.  
So effect of the ECT is 10%.  
So we've got this twice ER plus ECT multiplied by t where t is the nominal operating time of the downstream relay of the highest value fault current for downstream fault.  
We have to add to this, the circuit breaker operating time because of course for downstream relay when it operates sense a trip signal to the circuit breaker and the fault is not cleared until the downstream circuit breaker opens.  
During this time, the upstream relay still seeing the fault current.  
And our concern is that we've tripped the downstream relay and then almost immediately afterwards, we've initiated the tripping of the downstream circuit breaker and immediately afterwards we initiate the tripping of the upstream circuit breaker.  
So then we build in an overshoot because of course protection engineers are traditionally very conservative.  
So we build in a overshoot and we build in a safety margin.  
The overshoot is to represent the fact that when you have an electromechanical disc and you apply a current, once you stop the current, it does not instantaneously stop, it keeps turning for a short time due to the mechanical movement.  
And then we have a safety margin just to increase our confidence, our grading margins are correct.  
When you have a modern microprocessor relay, you have to think about things like a relay overshoot.  
You could design a microprocessor relay to have a zero overshoot because of course it has a, let's think of it as a virtual disc, a software disc.  
It doesn't have a physical piece of rotating metal.  
But of course what you often require in numerical relay is to grade with an electromechanical relay.  
So during this course, we'll begin to look at the problems of grading electromechanical relays with fuses and numerical relays with electromechanical relays or numerical relays with fuses.  
When we do, I've mentioned fuses and of course relays, the downstream relay probably has to grade with the fuse.  
So the fuse is probably located at the low voltage network and the relay is probably located at the high voltage, the 11kv network.  
So we have to now think about the relay fuse grading margin to ensure that the upstream relay does not operate before the downstream fuse because if the upstream relay operates before the downstream fuse, then the upstream relay will disconnect a lot of customers.  
And of course, the disconnection of many customers is financially costs money to the utility and as so, it gives reputational damage to the utility.  
So when it shows circuit fault is located just beyond the fuse, we have to think about, the grading margin.  
We have to assume again the source capacity is at its maximum level.  
The minimum grading margin between a relay and fuse is that mathematical expression, delta t = (ER + Ef) times downstream operating time plus the overshoot time plus the safety margin.  
Just going through that slowly.  
We got a relative timing error of the fuse of perhaps +/30%.  
So I'm worried that the downstream fuse operates slowly.  
So effectively, so it's affecting the downstream operating time by 30%.  
We've got a relative timing error in the upstream relay.  
So I'm assuming the upstream relay is going to go fast, so it's going to affect the time by 5% less.  
Then we have the nominal operating time of the downstream fuse for the value of current we pre-specify.  
This is maximum current seen for fault just beyond the fuse.  
And then we have the safety margin that's built into the equation.  
And we have the relay overshoot for the upstream.  
Every component has a maximum permissible time for which an overcurrent is acceptable, the higher the overcurrent, the smaller the acceptable time.  
And every component has a time-current characteristic.  
Remember, the objective of protection is to stop the component you're protecting being damaged.  
So the protection relay must operate and trip its own circuit breaker before the equipment you're protecting is damaged.  
A simple way of thinking about that is the cable to your computer in a British home, 230 volt plug sockets have a fuse within them.  
In the case of the lead to your computer, it's probably a one amp fuse.  
And the one amp fuse is really protecting the cable.  
So if your cable gets a short circuit, the fuse will blow.  
And reduce for risk of a fire.  
Alright so in the home it's about protect-...  
preventing a fire.  
And there's a legal requirement in the United Kingdom that every 13 amp plug must have a fuse.  
So whatever we're protecting has a time-current characteristic.  
And the characteristic for all the current values of the equipment we're protecting must be to the right of the protection fuse or relay curve.  
So remember what we're trying to do is to ensure that the protection fuse or relay operates before the equipment we're protecting is damaged.  
The talk was really about an introduction to overcurrent protection.  
What we're now gonna do is move on to more complex systems and look an example of overcurrent protection.  
So I hope this was a useful lecture and you're now beginning to understand the complexities of overcurrent protection.  
And I'll try and use an example to illustrate how to apply overcurrent protection in a graded problem.  
Thank you.  
  
  
  
# 2.2 Overcurrent Protection Example  
--LECTURER:  
Hello, I'm Peter Crossley.  
I'm a professor of power systems at the University of Manchester and director of the EPSRC Centre for Doctoral Training in Power Networks.  
I'm continuing the lectures I've given you earlier about Overcurrent Protection and Fuses, and I'm now gonna move in to a case of looking at examples of overcurrent protection.  
We're gonna spend this lecture now, looking at a particular example of how the grading study was done.  
We're gonna have to do a lot more examples, a lot more work in this area.  
Because you need to understand how to perform a grading study on a real radial distribution network.  
I'm gonna start with an example of an overcurrent protection study which was done many years ago.  
This is a system where we deliberately graded an entire system starting at 132 kilovolts with a fault level of 3,500 MVA through an overhead line into a transformer, then down to an 11kV system and down to a 3.3kV system.  
When you look my network, you can see the highest fault level is at first bar L, this is the start of activity, this is the source end.  
This is a 132kV busbar feeding 50km of 240mm squared overhead line, but has an impedance of 6.2 ohms.  
Then we have the next section from busbar K to busbar J, is a 30MVA transformer and we're going from 132kV to 11kV.  
Deliberately, to limit the fault current in this network, we have a leakage reactants to that transformer of 22.5.  
Generalising, leakage reactants in transformers vary from about 10-12%, in special cases, up to perhaps 30%.  
Then of course, we move to the next part of the network.  
Now we're down at the voltage level of 11kV and we've got 2km of 240mm squared paper insulated cable with impedance of 0.24 ohms.  
As we arrive at busbar H, the next section of cable is 200m, 120mm squared cable, again paper insulated cable.  
This is an impedance of 0.04 ohms.  
You must remember every busbar, there will be other lines coming of this, but all we're looking at is the part of the system that is relevant to the grading study.  
The diagram shows that busbar G is a 3.3kV system.  
It's supplied from a 4MVA, 11/3.3KV transformers.  
The 3.3kV system is assumed to be a rural network and is protected by fuses.  
This diagram is showing a detailed analysis of how we calculate all the impedances in the network in per-unit values.  
I'm gonna start off with the source.  
The source is at 132kV and its fault level is 3,500MVA.  
That means that if there's a three-phase short circuit fault at busbar L, the source will give a fault level of 3,500 of that, so the short circuit capacity is 3,500MVA.  
The base MVA value used in the per-unit calculations is 10MVA, so the source impedance is equal to 10MVA divided by 3,500MVA, which gives a source impedance of 0.0029 per unit.  
Next we have 15km of overhead line.  
When we convert the impedance value of 6.2 Ohms, we divide it by the base impedance.  
The base impedance is 132kV squared upon 10MVA.  
We get a value therefore, of 0.0036 per-unit.  
Connected between busbar K and busbar J is a transformer which is going from 132kV to 11kV.  
This transformer is 30MVA with a leakage reactant of 22.5%.  
We have to convert that value into per-unit based on a 10MVA base When we look them up, that will be multiplied by 0.225 per unit at the 30MVA value by the new MVA value which 10MVA divided by the 30MVA, and we get a new per-unit value of 0.0075.  
That makes sense, because originally it was a 30MVA at 22.5, so 10MVA, because it's a lower value, you would expect the new per unit value to be effectively one third.  
Moving on, we now have 2km of this paper insulated cable.  
The value of the 2km of cable was 0.24 ohms, if we convert 0.24 ohms to its per-unit value, we'll get an answer of 0.0198 per-unit.  
Remember, you take 0.24 ohms and you divide by the base impedance value.  
11kV squared divided by 10MVA is the base impedance value.  
Next we have 200m of cable between busbar H to the transformer, which is located next to busbar G.  
The cable translates to a per-unit value of 0.0033 per-unit.  
The big impedance value in this network is now the 11kV to 3.3kV transformers.  
In fact, transformers are what really limits the fault going in networks.  
When you go from 11kV to 3.3kV, the transformer is what changes the fault current value.  
In this case, the 4MVA transformer at 7% value translates to 0.07 multiplied by 10MVA divided by the original MVA value of 4MVA sort of base rating, so the rating of a transformer, and that gives a value of 0.175 per-unit.  
When you begin to put all those numbers together, and I'm deliberately gonna start at the bottom here and say busbar L.  
Busbar L has got a short circuit capacity of 3,500MVA, and of course, has an impedance at that point which is 0.0029 per unit.  
When we look at busbar K, the Thevenin equivalent impedance is 0.0036 plus 0.0029, and we get a value of 0.0065 per-unit.  
At busbar J, the impedance value, Thevenin equivalent impedance value for three-phase fault at busbar J is 0.0815 per-unit.  
At busbar H, it's 0.01013 per-unit.  
At busbar G, it's 0.2796 per-unit.  
What we now have to do is transfer these into short circuit capacity.  
The short circuit capacity at bus L is 3,500MVA as originally defined.  
The short circuit capacity at busbar K is 1,540MVA.  
At busbar J is 123MVA.  
You can see this big change as it goes from 1,540 MVA to 123 MVA.  
This is because of the transform of the 30 MVA, 22.5% transformer.  
The short circuit capacity at busbar H is 98.7 MVA and at busbar G is 35.7.  
Again there's a big change as you go from busbar H to busbar G.  
So you're going from 98.7 MVA to 35.7 MVA.  
If we now look at the fault current expressed over 3.3kV level.  
And of course, when we looked at busbar L, we're at 3.3kV level, the fault current is 610kA.  
If we express that over 132kV level, it would be 15.3kA.  
If we went to busbar K, the three-phase short current circuit at 3.3kV level and I realised we're now working sort of at 132 level, but from a per-unit perspective, my study's are really at the 3.3kV level.  
So, it's a fault current of 270kA expressed at 132kV, calculation it would be 6.8kA.  
At busbar J, it would reduce to fault level 3.3kA is 21.5kA and at 11kV is 6.5.  
At busbar H, it's 17.3kA and at 11kV level, 5.2.  
And finally at busbar G which is actually 3.3kV busbar, the current is 6.2kA.  
Looking at those values, we need to think about those values and the changes we're getting in the fault values as we go beyond the transformer in the network.  
This is showing the results from a grading study.  
The 3.3kV feeders are protected by fuses.  
So, they are protected by 200A fuses.  
So, I've drawn on this diagram first the 200A fuse.  
The highest fault currents seen by the 200A fuse is for a three-phase fault at the terminals of the fuse on the 3.3kV network.  
And that has short circuit capacity level of 35.7 MVA, which translates to a current of around about 6,000A.  
Then as we move up, we now do a grading between relay H and the 200A fuse.  
And that has been done.  
So relay H has been correctly graded to the 200A fuse.  
The grading is achieved at the point of 35.7 MVA and that is the grading margin.  
And then when we look at relay H for maximum fault level seen by relay H is a three-phase fault level of 98.7 MVA.  
And that again is the grading point between relay J and relay H.  
So when you go for...so we're going for this network step at a time.  
We start off with the 200A fuse.  
Then we correctly position relay H with respect of a 200A fuse.  
Then we position relay J with respect to the relay H.  
Then we position relay K with respect to relay H.  
Then finally we position relay L, which is the relay closest to the source with respect to relay K.  
When you look at relay L, the maximum fault level seen by relay L is 3,500 MVA.  
And relay L now is in a backup mode as a relatively slow operating time.  
So, this is a professionally done graded standard.  
And now we want to analyse how we can obtain these results.  
When we analyse that network, you can see that faults downstream of G, busbar G, the 200A fuse blows before relay H trips.  
So this is obviously correct.  
And the maximum current seen for fault at busbar G is 6.2kA.  
Relay H should trip before relay J for all faults downstream of H.  
And the maximum current for fault at H is 17.3kA.  
Relay J should trip for all faults that's between J and H, and it should operate before relay K.  
So the maximum current seen for fault at busbar J is 21.5kA.  
And relay K should trip before relay L for all faults downstream of K, and the maximum current for fault at K is 270kA.  
This is how we determine the grading margin.  
And of course relay L should protect the line between busbar L and busbar K.  
It's main protection and ideal at providing backup protection for a transformer located between busbar K and busbar J.  
The blue lines added to those curves are showing the main protection area.  
So, we're seeing how the main protection behaves.  
And we're seeing and the black line is really referring to the backup protection.  
So, I'm assuming that relay H is providing main protection from a fault level between 35.7 MVA and a fault level of 98.7 MVA.  
And relay J is providing main protection for faults with a fault level between 98.7 MVA and 123 MVA.  
Relay K is providing main protection for faults with a fault level between 123 MVA and 1,540 MVA.  
And finally relay L is providing main protection between 1,540 MVA and 3,500 MVA.  
And then of course what we're looking at the operating...  
When we look at that network, we can see that the main protection in all cases is achieving an operating time of less than one second, which sounds perfect.  
But the challenge is when you come to backup protection and whether the backup protection is inadequate.  
So, the operating time's achieved with these sections.  
For relay H achieves an operating time between 70 and 170ms for faults between H and G.  
Relay J achieves an operating time between 330ms and 420ms for faults between G and H.  
And relay K provides between 70 and 860ms for faults between K and J.  
And relay L provides an operating time of 250 to 390ms for faults between L and K.  
If we'd have done this study using definite time over current relays and if we'd assumed a margin of 300ms was adequate.  
And we could have set H to 250ms, J to 550, K to 850 and L to 1,150 so 1.15 seconds.  
This diagram is showing a mixture, so in the background in black is the inverse time characteristics And in the blue is the definite time characteristics, assuming we got high set a low set definite time.  
So, when you look relay H, we're using a combination of low set and a high set.  
The high set of course is an operating time of around about 0.25s, so 250ms.  
The low set of relay H has an operating time of 1s.  
In comparison relay J is a single element, so it has an operating time of 500ms.  
Relay K has an operating time of 800ms and relay L has an operating time of about just over 1s.  
So this is really the use of definite time discrimination curves when comparing definite time to inverse time.  
Then I'm now in this diagram.  
We're showing relay in the dark blue.  
The back-up protection times.  
And the real challenge in this network is the back-up time for relay L is unacceptable.  
So when you're looking at relay L which is protecting it's own section of overhead line plus the next transformer.  
In the case of a fault level of 123MVA, relay L has an operating time of greater than 100 seconds.  
So the relay located at L is struggling to see a fault on the 11KV side of a transformer.  
One option is to put a definite time characteristic.  
So I have redrawn this and I have inserted a definite time element set at 20kA primary settings.  
So this is a primary current setting with a 2s operating time.  
And you're seeing how that has improved the back-up protection time.  
But of course, in classical electromechanical relays, you would need a separate relay.  
When we're looking at coordination, the thing to remember is that you are trying to protect the equipment.  
So when you're looking at the characteristics of relay H and back-up relay J, they must be for protecting the 4MVA transformer.  
So the 4MVA transformer must be able toRelay H and back-up relay J must be for protectingmust be located below the transformer withstand characteristics up to 35.7MVA.  
This diagram showing some resultshowing instantaneous relays.  
So we're using the possibility of adding high set instantaneous relays to the IDMT characteristics.  
The original diagram you can see that the grading margins were 200ms between R2 and R3 and 150ms between R1 and R2.  
By adding instantaneous times, we can improve the grading.  
So we've installed effectively at relay R3, a 500A set instantaneous element.  
This allows us now increase our grading between R2 and R3 to 500ms.  
And then when you compare the grading time between R1 and R2, we've now increased it to 400ms by using the instantaneous element set at 1.4kA.  
Then for the relay R1, we've used an instantaneous element set at 3kA.  
You see how we've improved the grading study?  
Now I want you to almost play and I want you to study the system.  
So what we've done here is we've assumed we've got a very traditional power system.  
We've got oil circuit breakers and we've got electromechanical relays.  
The relative error of the relay is assumed to be 7.5 %.  
It's an electromechanical relay.  
The relative error of the fuse is assumed to be 30%.  
The CT error of the downstream CT is assumed to be 10%.  
The relay overshoot error due to electromechanical disc is 50ms.  
The safety margin we put into our network is 100ms and we are assuming the circuit breaker has an operating time of 100ms.  
We then go for the entire process of a grading study to work out the characteristics.  
And this is basic showing that the original study is really using this values and you can see the grading margins under the different conditions drawn on that diagram.  
And there's to be assumption this is oil circuit breakerstraditional oil circuit breakers and traditional electromechanical relays.  
If now we're to repeat the process, assuming we've got modern vacuum circuit breakers, and modern numerical relays, we would get a better performance.  
We've made some assumptions.  
We have assumed the error on the relay as a timing error is 5% of the downstream time value.  
Error of the fuse of course, still 30%.  
CT error still 10%.  
The overshootI put a small amount of 30ms overshoot on this numerical disc.  
It's a virtual disc.  
We could have put an overshoot of zero.  
It depends on the design.  
We built safety margins of 50ms and we are assuming the vacuum breaker has an operating time of three cycles.  
Again, we go through the grading process and we study what the outputs are.  
And this is showingSo you are seeing the old curves in black and we're now seeing the new curves in the colours.  
And you can see that the grading has now been improved and we're now get a faster operation performance.  
But still relay L when operating in back-up mode, has got maybe 20, 30s operating time.  
So the quest is, can we improve it more?  
And at this point, we begin to try different characteristics.  
So we're thinking well, could we have got a better performance using an extremely inverse or very inverse, as compared to the original standard limits.  
Could we have changed our plug settings?  
Could we have changed our TMS modes?  
And of course we are going for a process.  
We've concluded that standard inverse actually appears to be the best.  
But we need to be careful and we need to do this study.  
Nowadays this studies would normally be done using a computer simulator.  
But we are almost doing a hand grading study in this exercise.  
Continuing this examples, we're coming up with some protection setting.  
So the best solution for the relay at L is a standard inverse of a TMS of 0.2 and plug setting of 0.75Inom.  
So that when we look at this, this is assuming there's minimum back-up protection times in the original ones where we've put a definite time in.  
These are showing the characteristics of standard inverse definite time.  
Very inverse, extremely inverse on the curves.  
And now this is showing the results for relay L.  
So I'm concentrating on relay L and am considering what would have happened if I'd have changed the changed the characteristics.  
So am going fromI'm trying extremely inverse, very inverse standard inverse to produce a better performance.  
And I'm trying different plug settings of 100%, 75%.  
I'm continuing with process now.  
On relay K, I've put an instantaneous element, which has allowed me to bring relay L down.  
It's allowing me to set relay L at the setting of 75% with a plug setting of 0.1 and you can see how significantly improved the performance in the backup protection mode of relay L.  
So in the backup mode we've now got an operating time of less than 10s.  
The lecture I've just given is really a basic introduction to overcurrent protection and how overcurrent protection works on a radial distribution network.  
My subsequent lectures will begin to look at more complex networks and we'll look at various examples of how you create a system.  
I hope you find it interesting.  
Overcurrent protection I believe is the most important protection on a power network and it really is what keeps the lights on on our distribution networks.  
Thank you.  
  
  
  
# 2.3 EPSE Overcurrent Protection Tutorial  
--Hello, I'm professor Peter Crossley, professor of power systems at the University of Manchester and I've spent my entire working career involved in the protection of power systems.  
I'm going to go for question one in your tutorials question sheet which will now give you a work solution to that question and I will then discuss some of the issues the question raises.  
So what we've got is we have as a power system where we've got a 3.3 kilovolt busbar which has got a fault level of 100MVA.  
So that's for main supply busbar.  
I'm going to number this busbar as number three.  
And leaving the busbar, we're going to do the protection study on just one feeder.  
Obviously the real 3.3 kilovolt busbar will have many feeders coming off it.  
But we're going to look at the protection of one feeder.  
I'm going to refer to this as relay B and the impedance of this feeder is 0.2 ohms.  
And then as you move down downstream through the network, you get to the next busbar.  
And again, I'll just draw this a little bit thicker so you can see it is a thick busbar and then at this point, I'm going to put circuit breakers here and here.  
These two branches are identical.  
So when I look at this one, this is basically relay A.  
I'm going to refer to this as busbar two.  
And then connected on both these feeders, are two identical transformers.  
And these transformers then go to a next busbar.  
This is dropping down to the 415V supply and it's the same on both sides.  
So it's gone from a 3.3kV to a 415V.  
Each of these transformers is 500 KVA, with a leakage reactance of 7%.  
So again, 500 KVA and a 7% leakage reactance.  
And then coming off these feeders, I've assumed these three LV feeders which are protected by a fuse, these are high rupturing capacity fuses.  
So in many senses, this is similar to the system supplying where you live.  
So of course down your street, there's a three phase cable which is generally protected by about a 600 Amp fuse.  
In this case, we're protecting them, each of these fuses is a 450 amp fuse and of course, these are three phase connections to sets of houses.  
So if you looked at your own individual dwelling, it would have a single phase to one house and perhaps your neighbour has a second phase and your following neighbour a third phase.  
Traditionally we tried to balance the system.  
The protection relay is here and here.  
And of course, what we're going to look at is the grading of relay A versus a fuse and then relay B versus relay A and we're going to make sure that we adequately protect the network.  
The objective is if a fault occurs here, so if we get a fault at this location, we expect the fuse to operate.  
If for some reason the fuse is unable to operate, then this would provide backup.  
But actually the main objective of relay A is to protect the transformer.  
So this feeder to the transformer.  
And then of course, relay B is here to protect this section of cable and then provide backup to the next system.  
This is a classical philosophy of overcurrent protection so that a single failure does not cause an inability to clear the fault.  
The operating behaviour of this simple relay, so the simple over current relays correspond to an equation I squared T equals K.  
So in fact we could rewrite that and we could write it as T equals K divided by I squared.  
And of course, this has now got a squared relationship and what it's showing is as the current increases, the relay goes faster.  
So if the current was to double, the relay would go, would operate in a quarter of the time.  
If the current was to go up by factor four, the relay would operate in at one 16th of the time.  
So it's got an I squared characteristic.  
For the example, So I in this example is primary current and it's at 3.3kV level.  
So it's basically the current that flows here, the current that flows here cause that's what we are predominantly interested and we're checking that this relay will grade correctly with the downstream low voltage fuse.  
The time is the operating time of relay in seconds and K is a constant which is equal to an integer.  
So it's an integer multiple of 10 to a five amp squared seconds.  
So it's effectively, it's a value of say L where that's an integer multiplied by 10 to the power five and the units of this is amp squared second from the equation.  
So of course, what I want you to do is to determine the settings in primary amperes for the overcurrent relays at A and B.  
I'm just going to mark this again cause on my recording it hasn't taken that up, so we'll put A in there and then we're now going to go through the answer.  
The starting point is this is a 450 amp fuse and we're given some values in the question.  
Which said this 450 amp fuse is approximated by an operating time of 10 seconds at three kilo amperes and this is on the LV side.  
It also has a current of 2.5 seconds at four kilo amps.  
So as we increase the current, the fuse operates faster.  
Fuses are wonderful in clearing a very high current fault but tend to be much slower on low current faults.  
And in fact fuses are the most popular protection device used but of course, they're mainly used at low voltage.  
And then if we move down and the last one is 0.02 seconds.  
I've just got a limited number of points which we will then plot on a logarithmic diagram.  
And then we, another piece of information, we have the minimum grading margin between the relay and the relay and the relay and the fuse.  
So the minimum grading margin, and I've made an assumption because obviously it was a tutorial question to make it easier.  
I've made the same assumption for relay to relay grading, and relay to fuse grading.  
So the minimum grading margin satisfies this equation, delta T equals 0.2 times T plus 0.3 seconds.  
So that means the minimum grading time would be point three of a second but then you need to add to it this 20% of the downstream operating time where this refers to the operating time of the downstream device.  
Okay, I'm going to start by describing the transformer and I need to calculate its ohmic value in ps.  
So the Z of each of these transformers so this is a 500 KVA, 7% and that is now going to be equal to 0.07.  
So I've converted the 7% reactance to a per unit value and then I've multiplied by kilovolt squared upon MVA.  
So use this equation kilovolt squared.  
So what I'm doing is effectively taking the X l multiplied by kilovolts squared upon MVA.  
So of course in this case, what we've got is 3.3 squared divided by 0.5.  
That's a transformer is equal to 500 KVA which of course means it's 0.5 MVA.  
So as I put the numbers into this, I end with a value of J, so it's imaginary cause it's a complex number.  
It's a reactance of 1.525 ohms.  
Because it's a tutorial example, I'm going to put three decimal points.  
If you were doing this in a real system you'd probably put just one or two decimal points.  
So then I'm going to look at the 3.3 KV equivalent source equivalent fault level.  
That means the three phase fault level and that is equal to a hundred MVA and therefore Z s at that fault level is equal to kilovolt squared divided by MVA of the fault level.  
Remember, it's three phase fault level which is going to be equal to 3.3 kilovolts squared divided by 100 and that translates to J 0.109 ohms.  
So the ohmic value of J 0.109 ohms.  
I'm now going to redraw the diagram in a simplified form.  
So what we've got, we've got the source.  
So which is 3.3 kilovolts source but when we consider the line to neutral, we get that value.  
And then we've got the source impedance to busbar three so this is the hundred MVA source impedance.  
So we've got a value of J 0.109 in ohms.  
Then of course, and this is where the first relay is located.  
So this consists of relay B and then we've got another impedance which you were told in the question is J 0.2 per unit.  
Sorry I made a mistake already.  
It wasn't J 0.2 per unit, it was J 0.2 ohms.  
So it's an ohmic value.  
And then we go from busbar two to busbar one and this impedance here is J 1.525 ohms.  
And then at this point, we come to the fuse and we now will let the LV so.  
But we're studying all this as if it's a 3.3 kilovolt system.  
If we look now at the fault current and we can see that downstream of a fuse so at this point, we need to put fault here and it's basically a three phase fault there.  
So three phase fault, we will get a current.  
So this is downstream.  
So if we're sitting at this fuse, that's downstream and this is upstream.  
If we're sitting at relay A, this is downstream, this is upstream.  
Relay B, this is downstream going down the network and upstream back into the grid system.  
So downstream of a fuse I is going to be equal to 3.3 kilovolt, this is referring all to 3.3 kilovolt side and if we add all those numbers together, so J 0.109 plus J 0.2 plus J 1.525, we get a value of J 1.834 which calculates the 3.3 kilovolt level of 1.039 kilo amps.  
So just over a kilo amp is the fault level of a current that will flow into a solid zero fault at that location if it was a three phase fault.  
We can also translate this into the LV side.  
So the I of the LV, which of course is the actual current which would flow into actual fault at that point is equal to 1.039 multiplied by 3.3 kilovolts divided by 0.415 and that gives us an answer of 8.3 kilo amperes.  
So we get an answer, 8.3 kilo amps when expressed at the LV side.  
So faults downstream of busbar one are protected by a fuse.  
So faults downstream of busbar one are protected by the fuse.  
And this is of course normal procedure on the L V system.  
Now remember the current values we had for the fuse, the operating times.  
we need to translate those into the, the 3.3 kilovolt side.  
So if we looked at the fuse.  
The time of the operation of the fuse when it goes in 10 seconds.  
corresponded to three kilo amps on the LV side and if we convert three kilo amps and we do this by multiplying 0.415 divided by 3.3 multiplied by three kilo amps.  
So this is now on the 3.3 kilovolts side.  
So when we refer to 3.3 kilovolt, it gives an answer of 0.377 kilo amps.  
Remember that is it 3.3 kilovolts we've referred it to 3.3 kilovolts side.  
If I now look at the other values, so for a value of 2.5 seconds which corresponded to four kilo amps on the LV.  
This translates to 0.503 kilo amps on the 3.3.  
If we now go down, so 0.3 seconds, corresponded to six kilo amps on the LV or is equal to 0.754 kilo amps on the 3.3.  
And then if we move down further, so 0.07 seconds corresponded to 8 kilo amps LV which translates to 1.006 kilo amps on the 3.3 and on the last one in the example of a fuse, 0.02 is equivalent to 10 kilo amps LV, which is equal to 1.257 kilo amps on the 3.3.  
So this is a 3.3kV side.  
At this point, what I would normally recommend to students is you draw a fuse characteristic on the log graph on the logarithmic graph paper.  
Obviously in an exam situation, you will be given an appropriate level of log graphic paper.  
Regrettably 'cause I'm working on a white board, I do not have a log graph paper.  
So you're going to have to just accept a little bit my values and I'm going to try and draw the characteristic of a three cycle by three cycle log graph plot.  
And of course when I do that, remember it's logarithmic.  
So what you're doing is, these should be equal.  
So these are like, so this actually when we put the values into it, this would be 0.1 kilo amps.  
This would be 1.0 kilo amps, this would be 10 kilo amps and this is going to be 100 kilo amps on these units and that's a three phase fault level, fault current.  
And remember these are logarithmic.  
So if you were to draw these, you discover that this would be 0.2, this would be 0.3, 0.4 and of course it's going logarithmic.  
So 0.2 0.3 and all the way out to one but it's a logarithmic scale.  
It's very difficult to do on a screen.  
In the same ways, when I look at the the the Y axis, again it's three cycle by three cycle.  
So what I'm going to do is try and draw.  
So I'll put that one there then another here and another here.  
They are meant to be equidistance.  
So I'm going to call that 0.01 seconds.  
So that of course is 10 milliseconds.  
So if a protection was operating 10 milliseconds, you're saying the protection is operating in half of one cycle of a 50 Hertz waveform.  
This is a hundred milliseconds.  
This is one second and this is 10 seconds.  
And now what I'm going to do is draw on the diagram as best I can and I'll show you the example I've done separately against these values.  
So of course if I was to continue this one up here and I realise it's very difficult to draw this.  
I'm going to end up with a characteristic for the fuse.  
I'm going to draw the various points on the fuse which are quite difficult to draw and draw on here.  
I'm going to put one up here and I'm going to connect all points together and I'm going to get a fuse characteristic that will look something like that when I plot through the points.  
And that really is the 450 amp fuse, which of course you have to draw correctly on the log paper.  
So let's go back a bit.  
So I've drawn the fuse characteristic and now what I'm thinking about is the grading of a relay against a fuse.  
So the first thing I try and do is determine what is the maximum value of the current.  
And in this case, the maximum value of the current for a fault that's downstream of the fuse is the maximum rise from the terminals of fuse is 1.04 kilo amps.  
So I'm going to stop my characteristic there and I'm going to say this is this is I maximum for LV fault, so for low voltage fault.  
And that was calculated earlier at 1.04 kilo amps and it's at this location here.  
And then what I'm going to do is calculate the grading margin to the next relay.  
So I'm going to calculate those values and I'll show you now how to do that.  
So maximum I for the fuse, so this is a three phase fault that's downstream of a fuse and it has a volume of 1.04 kilo amps.  
The full current maximum I fault for a fault at busbar two works out at 3.3 kilovolts divided by root three divided by J 0.309 (coughs) and that translates to 6.166 kilo amps.  
And then for the maximum I F at busbar three, again 3.3 kilovolts divided by root three divided now by J 0.109 and we get an answer there of 17.48 kilo amps.  
So you can see as we get nearer and nearer the supply, the grid supply point, the fault current increases.  
And when we look at the fuse at I F equals 1.04 kilo amps, it operates in five milliseconds.  
So 0.05 seconds, which of course is the value on this point here.  
So this is the operating time of 0.05 seconds for the fuse when it's got the maximum current passing through it which is a solid three phase fault.  
I use the term solid to affectively describe what is almost like a bolted fault.  
It's a zero ohm fault.  
And now we begin to look at the grading issues.  
So relay to fuse grading and this is the grading margin is equal to 0.2 times the downstream operating time of the fuse.  
So it's the time of the fuse at this value of current of 1.04 kilo amps.  
So effectively it comes out at 0.05 seconds and that's plus the margins of errors of 0.3 of a second.  
In the lectures, I've sort of described this in slightly more detail of why we have that value of point three.  
These are values typical for electromechanical relays.  
And then if I put the numbers into here, I get a value of 0.31 seconds.  
So that is the grading margin at this point.  
So I have to make sure that I do not go beneath the grading margin.  
So the minimum operating time for relay A for a fault at the fuse and this is for a fault at the fuse.  
So this is on the LV side is going to be equal to T equals 0.31 seconds plus 0.05 seconds which gives 0.36 seconds.  
And now of course we now have to think of a value of K which we use to calculate it.  
So looking at relay A, we can see that K is equal to I squared T.  
So I is equal to 1.04 times 10 cubed, all squared because of this characteristic multiplied by the minimum time.  
So this is really a minimum, so we take a value of 0.36 and when I put the numbers into that I get an answer 3.9 times 10 to the power of five.  
I was told originally we can only have integer values of K where it's integer values are the multiple of 10 to the five.  
So I select K is equal to four so 4.0 times ten to the five and this is the value of K I've chosen for my first relay.  
The interesting one, one of the things we haven't yet discussed is the problem of inrush current.  
So when you first energise a transformer, you get an inrush current and obviously it's important that the protection does not operate during inrush.  
So what I now like to do is to check whether if we did have inrush into a transformer, would the protection remain stable.  
So this point I'm going to wipe off this part and now discuss the argument of inrush.  
I'm going to take some typical examples so you can begin to think about the problems of inrush and protection maloperation.  
The question, the exam question itself did not mention this.  
So really you could ignore it but in a real problem, it would be correct to take it into consideration and obviously if the exam question had included it, you must consider the inrush of the transformer.  
Okay, the question didn't mention the problem of inrush when you energise a transformer but obviously in a real situation when you first energise a transformer, you get an inrush current.  
Which typically the inrush current generally looks something like that and it will slowly decay down.  
This goes on for a long way, so it goes on for a long time.  
You get these spikes of current which flow into a transformer when you first energise it.  
But protection must not operate on that because that is the normal behaviour of a transformer and it's referred to as inrush.  
In this exam, I'm just going to begin to think a little bit.  
So let's say, let's just assume.  
We've got an inrush which is equivalent to seven times the full load current.  
So seven times the full load current, and I'm going to save the inrush is present for less than one second and after one second due to resistance in the transformer, it's decayed away.  
So we've got one second of inrush.  
We're going to start by that.  
So the question is now, if we look at seven times full load current, the full load current is equal to 500 KVA divided by three times 3.3 kilovolts.  
This is the equation you've learned in other parts of the course which gives an answer of 87.5 amps and that's a full load current.  
So seven times, so the inrush is equivalent to a value of 612 amps.  
So the question now is what happens?  
So if we look at the operating time of relay A of that value of current, I'm assuming it's present for one second, we get a value of four point nought times ten to the five all over 612 and that's squared.  
And actually when we put the numbers into this, we get a value of 1.07 seconds.  
So what that means is the relay will not operate unless the inrush continues for greater than 1.07 seconds.  
So of course this was a guess and of course inrush depends on the design of the transformer is it a low loss transformer, it's core design.  
So if we just said, if for example, if the time of inrush was equal to two seconds, we have a problem because at two seconds, our protection would not remain stable and would falsely operate.  
So let's just, let's just for example let's increase K in this case to equal to eight times ten to the five.  
So of course when you look at this we make that number eight.  
So then of course the operating time of relay is now eight point nought times 10 to the five divide by 612 squared and at this point we get 2.14 seconds.  
So now we know that this will be stable with this new value of K.  
Well, the problem is as we bring this K value up, it means we move the characteristic upwards and when we begin to create relay B against it, we may have another problem.  
So I'm going to start by running it with a value of this one.  
So I'm going to actually now rub this off and forget about it for now but we turn to it.  
So is this recorded, So yep.  
So I'm just going to take that away and we were going to assume that we do not need to worry about inrush.  
The settings we've calculated were adequate and the value of K is adequate.  
So at this point what I'm now going to do is work out what it means.  
So I'm assuming K is 4.0 times ten to the five.  
So actually let me get rid of all this because we know that it has not falsely operated on inrush.  
Let's continue the derivation of the next lot of settings.  
Obviously if the exam question asked about inrush, you should take it into consideration.  
If we didn't mention inrush, it would look good in an exam question to say you have to be worried about inrush into the transformer and and you should try and do calculations to determine that the Protection will remain stable in the energisation of the transformer.  
So we're going to start by saying that K on relay A K is equal to 4.0 times ten to the five Say that again.  
I'm resting my arm, Yeah.  
Exactly yeah.  
I'm sorry.  
Yeah.  
That's okay.  
Okay, so I'm going to start by writing the equation for relay A and K is equal to 4.0 times 10 to the five amp squared seconds.  
And now I'm going to start putting some numbers because of course what we want to do is plot the values.  
So the first one at 1.04 kilo amps.  
So remember this is this case, this is a case of 1.04 kilo amps.  
I want to calculate the actual operating time.  
So at 1.4 current the relay operates a 4.0 times 10 to the five divided by 1.04 times 10 cubed all squared which gives them answer of 0.37 seconds.  
So this value now goes onto my curve and on this curve, and I apologise you need to do this on log log graph paper.  
But if we look on here, I'm going to assume that it operates here and that's my value and that grading margin is now adequate.  
So that's for first point I've put on my curve for relay A.  
Now I'm going to look at other values.  
So at downstream of relay A at busbar two where we get a value of 6.166 kilo amps.  
This is the current we calculated and the operating time 4.0 times 10 to the five divided by 6.17 times 10 cubed all squared and the answer I get there is an operating time of 0.01 seconds.  
So if I come down here, the next point on here it's a value of 6.166 kilo amps.  
Remember this is a logarithmic scale.  
So 6.1 is probably around about here.  
So my next point is 10 milliseconds.  
So we're now going to start drawing another curve.  
I need obviously more than two points to draw our curve.  
So at this point I'm going to calculate some more at three kilo amps, T four point nought times ten to the five divided my 3.0 times 10 cubed all squared which gives us an answer of 0.04 seconds.  
So I can go onto this one and I find my curve three kilo amps which is probably about here and I get a value of a 0.04 so somewhere around here and of course I'm beginning to get my line forming and then I'm going to take a few more, six kilo amps.  
Sorry, at six kilo amps on the LV, So I'm interested in how is the relay performance backing up the fuse which corresponds to 0.754 kilo amps on the 3.3 kV.  
So I put those values into here and time is equal to 4.0 times 10 to the five divided by 0.754 times 10 cubed all squared which gives me an answer of 0.704, so 0.7 seconds.  
So I come along here and a value now of 0.754 which is probably somewhere around here.  
I get about 0.7 seconds so I'm probably just right up here and actually what's interesting, I'm beginning to see this curve is going up and it's beginning to look as if it might cross.  
And I'm interested in not crossing because actually when you begin to get the cross, what it means is the relay will operate faster than the fuse.  
So if you downstream of the fuse there's a low voltage.  
So there's a low current fault, the relay will operate first and disconnect all the feeders connected to the busbar.  
So multiple customers will lose supply which of course is not advisable because financial compensation is paid when customers lose supply.  
So there's now let's just look at another one at four kilo amp LV just to prove this fact.  
So it's 0.503 kilo amps on the 3.3 kilovolts side and then T 4.0 times ten to the five divided by 0.503 times 10 cubed all squared and I get an answer there of 1.6 seconds.  
So now at 1.6 seconds at a value of 0.5 so 0.5 is probably somewhere about here.  
So a value of 1.6 it's probably a value of that here.  
So you can see I've crossed.  
It's not perfect but that's what the grading study is giving us.  
So the relay A can operate faster than the fuse for full current of less than four kilo amps on the LV feeder.  
So this is a problem.  
And of course when you're writing an exam question, it's really important to think about what the solution means.  
Here again.  
Can It be right.  
(laughs) Adding a problem to a problem.  
Problem yeah.  
So the relay A operates faster than the fuse for a fault current on the LV side, this is what is marked as it's downstream of a fuse.  
So on the LV side of a value of four kilo amps but on the LV side.  
So it's four kilo amps on the LV.  
Remember we got a 450 amp fuse.  
So we're talking about sort of several times the rating of a fuse.  
Remember when you think of fuses, fuses operate very fast at 10 times folk ohm but as you begin to get less than that, begin to go slower.  
So we've got, we've got this challenge really with grading.  
So now what I'm going to do is continue now to begin to look at relay B.  
So we're going to continue.  
So we've drawn on here this is relay A and of course it's much neater when you draw it on a log log diagram.  
So that's the original fuse and relay A and now we're beginning to look at the maximum current we get for fault.  
Do that again Peter cause it hasn't come through On it's relay A.  
Yeah, please.  
So just to emphasise, this curve here is relay A curve and now what I want to calculate is where relay B curve would be where it would be on this diagram.  
When we look at relay B, it needs to coordinate with relay A up to 6.17 kilo amps.  
So this could have relay B coordinates with A up to 6.17 kilo amps.  
That's the maximum current that is seen downstream of relay A.  
Just do A but not the other side.  
That's it.  
The operating time, so a T operational relay A at 6.17 kilo amps is equal to T equals 0.01 second, which is this value here.  
That's the value.  
And the relay B to A grading margin, the time is equal to 0.2 times 0.01 plus 0.3 which is equal to 0.302 seconds.  
Therefore, the minimum T up for relay B at 6.17 kilo amps is equal to 0.31 seconds or 0.312 seconds to be precise.  
So we need to select a value for K.  
So remember K equals I squared T which is 6.17 times 10 cubed all squared times 0.312 and when we calculate that, we get an answer of 119 but I'm going to choose 120 times 10 to the five.  
I'm just going to round up very slightly to 120 times 10 to the five.  
That's the value of K I'm going to select.  
And now of course what I'm going to do is start calculating the points on the curve.  
So at I is equal to 6.17 kilo amps, T is equal to 120 times 10 to the five divided by 6.17 times 10 cubed all squared which is equal to 0.315 seconds.  
You can see slight, very slightly longer than we had before.  
So we've got, we've got the margin is acceptable.  
If I continue this and am not going to write over derivation at 1.04 kilo amps, you get an operating time of 11.1 seconds.  
At 10 kilo amps, I'm just trying a few numbers here to get some points on my equation.  
The operating time is 0.12 seconds.  
At three kilo amps, so I've just got a few values in so I can draw my curve neatly.  
I can put lots of points on I get a value of 1.3 seconds.  
At 0.754 kilo amps, T is equal to 21.1 seconds and at 0.503 kilo amps, obviously I select these values because these are the values that we used before.  
I get a value now of 47.4 seconds.  
I then begin to draw these values so for example, at 0.503, I'm getting an answer of 10 seconds.  
Okay, 10 seconds.  
Actually in this case now I'm above the top of the curve, so I'm somewhere up here from this value of that and at that point I would have a 0.503.  
So a very long operating times it will appear.  
So I'm happy this one 21.75 up here.  
So I'm getting basically a curve which has got the, let me mark the grading margin off first, let me go back to find where I was.  
So this is a value of 6.17 , 0.315 So I come up from here, this remember is the value point is the value of, I'm losing my point.  
This is a value of 6.17 kilo amps.  
And I come up there, I put the grading margin.  
So I come up to 0.3, which is somewhere around here and I draw my next curve and I start my curves down as I go down to here 0.315.  
I go to this one at 10 kilo amps which 10 kilo amps is here.  
10 kilo amps, I get a value of 0.12.  
So somewhere here, here and I draw all those curves I draw the curve and I get something like this so this is the curve for relay B.  
Okay, so we've really completed the exercise obviously it's easier when you've got log log graph paper.  
For the last part of the question and that was sort of a question really is saying, finally assess whether the relay at B provides adequate backup protection from the transformer normally protected by the relay to A.  
(coughs) So when we looked at the network diagram, did the relay at B provide adequate protection?  
And of course what we're beginning to see is backup to relay A cause we're really looking in this area.  
We're beginning to get slow operating times.  
Slow operating times in maybe 10 seconds and again you need to calculate these and those are really not acceptable.  
So what are our options?  
What could we do?  
So how could we improve the performance?  
One option is we buy another relay.  
We purchase a different relay and perhaps we set a relay here.  
So we add another characteristic which is a definite time characteristic.  
So one option is to pick a definite time characteristic to add to our inverse characteristic.  
In that way, we get something that looks like that.  
And what that really means is that the maximum operating time for relay B is one second.  
So it gives greater protection for the transformer.  
What I've done, I've given an example of a grading study using a whiteboard and really I will give you then my final answers which will be added to the notes and my final grading.  
You probably cannot see this, but I came up with a diagram that looked to that form.  
this will be added to the results.  
This one I deliberately did for K equals four times 10 to the five and you can see on the diagram, I added a definite time relay set it to current value of greater than one kilo amp and with an operating time of one second.  
And then I repeated the process and I said, well, let's just assume that we've got an inrush that's lasting for too long.  
So I've assumed the inrush is two seconds and of course with the value of K equals four times 10 to the five.  
The relay would have falsely operated on the energization of the transformer.  
So I've re-drawn the grading diagram.  
Again, I've added a definite time.  
In this case, I've set it to two seconds operation and I've again set it for an operating current of greater than one kilo amp.  
So thank you.  
I hope this helps you understand how to do a grading study and this example was a useful exercise and will hopefully help you in your exams, and your future careers.  
Thank you.  
  
  
  
# 3.1 Differential Protection Of Feeders  
--LECTURER:  
Hello.  
My name is Peter Crossley.  
I'm professor of Power Systems of the University of Manchester.  
I'm here to talk to you about Power System Protection.  
This lecture is about differential protection, but it's differential protection applied to feeders or lines cables.  
So I hope you enjoy this talk on differential protection applied to feeders.  
There will be other lectures and other aspects of differential protection.  
Differential protection is one of the best protection techniques we have, but of course, relies on communications between the two ends of the circuit as you will see in these slides.  
So thank you.  
Differential Protection of Feeders, so this is lines and cables.  
Differential protection is a preferred option because it's often difficult to apply overcurrent protection particularly to transmission lines, and distance protection are some limitations when applied to transmission lines.  
In fact, the National Grid in the United Kingdom, their first main protection is differential protection.  
The second main protection is distance protection, and the backup protection is a combination of distance and overcurrent protection.  
So differential protection is a very important role in the protection of transmission feeders whether it's overhead lines or underground cables.  
You can achieve fast fault clearance with differential protection for all parts of a protected plant.  
When you look at the behaviour of all the current protection as the fault current becomes low, the overcurrent protection times become very long.  
Differential protection means fast maintains fast operating times for positions of all faults in the networks including low current faults.  
So it can be used to protect all items at plant, generators, transformers, feeders, busbars, motors.  
It's a very effective form of protection.  
In fact, in my opinion, it is the best type of protection we have.  
Differential protection forms a defined zone of protection which is basely dictated by the location of the current transformers.  
So we're basically protecting a zone which is between the current transformer.  
This is showing a very idealistic diagram, so we've got a network where the power is flowing from the source to the load.  
And of course, under that condition, we're protecting that feeder which effectively is with the section of feeder between the two current transformers.  
So when we look at that diagram, we can see that we've got current transformer on the right, current transformer on the left.  
On the secondary circuit which is drawn in the thinner lines, what we're seeing is that the current flows into a relay, so a relay's connected across the source CT and the load CT.  
And affect the current that flows through the relay is the difference between source current and the load current.  
And CTs are connected in such a way that IR is equal to I1 I2.  
So in that diagram, relay current should ideally be 0, so under normal load conditions, there should be no current through the relay operating coil, and the protection relay should remain stable.  
During an external fault, there should also be no current flowing through the relay coil and the relay should remain stable.  
But later, I'll illustrate some of the difficulties in achieving that.  
When you have an internal fault, of course, looking at the diagram, the current flows from both ends into the fault, so it flows effective from the source into the fault or from the load into the fault, or of course, if there's no sources in the load, it will just flow from the source into the fault, and suddenly, you have a current now flowing into a relay which is the fact that the current entering at the source, end, is not equal to the current leaving at the load end.  
These protection systems can be set to operate very quickly and consequently they're a very effective form of protection.  
There are two types of differential protection used for feeders.  
There are high impedance techniques and there are low impedance techniques.  
The high impedance techniques are based on what is referred to as the Merz-Price circulating current principle.  
So it was actually almost first developed in Newcastle in the United Kingdom using these techniques.  
Probably 70 years ago.  
To operate this high impedance differential protection schemes, you're required much current transformers below reactance designed, and these are referred to as class X or equivalent CTs.  
This is described in a very classical form of protection which is very successful, very important form of protection, very widely used, and it's actually been used for, I guess, 70 or 80 years.  
You have equal CT ratios.  
Most really importantly, becomes much easier if you use the same ratio CT.  
Your major problems if you do not do that.  
You have a current operated relay with an external stabilising resistor.  
So we begin to introduce this issue of stabilising resistors.  
Then, we also connect cross stabilising resistor in the relay and non-linear resistor which is limit required to limit the fault current.  
We often refer to these as Metrosils and these are non-linear resistors which basically conduct and protect the relay when it's high voltage, so they're really there for protection of the relay from damage in the case of an internal fault.  
They only have to operate to bypass for current in the case of internal fault.  
High impedance differential protection is very simple design.  
Can be used for zones of protection up to a few hundred metres in length.  
As you get beyond this line for capacitance effects of the secondary or often referred to as pilots, becomes so significant that we begin to get problems of imbalance currents flowing.  
This is showing a circulating current system of a very idealistic system.  
And what we have is a system where we got NG and NH.  
So coming out of a CT of the ideal CT and NG is a secondary current which is the primary current divided by the turns ratio.  
Of course, then we have the excitation current.  
It's flowing through the magnetising branch of the CT and NG.  
We have the opposite effects at NH, so at NH, we have the excitation curve is flowing through the magnetising branch of the CT at NH.  
Then we have the circuit.  
RSG refers to the CT winding resistance of the NGCT.  
RLG refers to the lead resistance of a connecting leads causes a copper connecting leads generally twisted pair leads to connect the CT to the relay.  
87 is the differential.  
This is using the American terminology for differential relay as defined by IEEE.  
So very effective notation, the IEEE numbering system for relays.  
Then we have a stabilising resistor, in that diagram is RG.  
And we also, of course, at the other end of the NH, we have RLH to be the lead resistance.  
RSH to be the CT wiring resistance.  
We have ZEH to even magnetising impedance of the CT.  
If both CTs have got the same magnetic behaviour of the same currents for an external fault.  
Generally, the issue is often about external fault.  
Then at point J, there is no voltage.  
This assumes two identical CTs and pilot circuit, so on this external case, there's no voltage at point J.  
When you look at that system you begin to think, "What would happen if we have of course had a different magnetic history of the CT?" So if one CT had got various effect within the CT And consequently rapidly discovered, this was done many many decades ago, that this approach has major limitations.  
So by the fault, we began to think about alternative methods, and we used this technique which solves the problem of transient instability.  
So what we do is now defined as a high impedance differential protection scheme, and we actually begin to assume our analysis assumes that one CT will be completely saturated.  
So when we look at our system, we can see that V = I1 x Rlh + Rsh and that voltage V.  
So looking at the diagram, you can see that the voltage across the relay and the stabilising resistor.  
If the CT end H is fully saturated, that means there's no output current from end H.  
But current now, V equals I1 times RLH plus RSH But V value, so, the voltage across the relay and the stabilising resistor.  
Now, of course, creates a current IR.  
So, IR is equal to V divided by the resistance of the relay.  
So, R 87, plus the resistance of a stabilising resistor R, R.  
So, when we, of course, the resistance of relay is very, very small compared to the stabilising resistor.  
So, in fact we can simplify that down, so, the current flowing is equal to I1 times RLH plus RSH divided by R, R.  
So, is equal to V upon R, R.  
So, what we've done in that system, if we've assumed the relay impedance alone is to low to ensure stability, and the relay circuit impedance can be increased through the addition of an external resistor which is it connected in series with the relay, the required circuit impedances, R, R, must be greater than V divided by IR.  
To prove that under the worst external fault condition, we maintain stability.  
When we do the calculations for determining the stabilising resistor, we take the worst case external fault current, so, the highest external fault current.  
Perhaps we might even take the circuit braking capacity to define the maximum fault current.  
And then we assume that one CT is completely saturated and then we calculate what the voltage will be across the relay and the stabilising resistor, if we need a stabiliser resistor.  
But voltage, then what we try and do with the stabilising resistor is to reduce the voltage, so, reduce the current, the flows through the relay 87 to a value that's below the operating current of the relay, so, the relay does not operate for an external fault condition.  
When we move to a low impedance differential protection scheme, the current transformers are connected in series with two relays in that structure.  
We've crossed them over to ensure that the currents effect on an external fault oppose each other, so, in the case of an external fault, no current flaws.  
So, there's no current flow for an out of zone fault.  
The stability limit of voltage balanced schemes is very low, so, that required us to begin to use high impedance differential schemes.  
The problem with a high impedance differential scheme is we have to be able to communicate the current from one line end to the other line end, and that can be very difficult, therefore we move to techniques using low impedence protection schemes.  
This is showing the structure of a low impedance bias differential scheme.  
where we've got bias currents and operating currents.  
And the differential current versus the through current, the average through current, you have this characteristic, if you're above the line, you operate, if you're below the line, you restring.  
And so we have these elements in electromechanical relay where we have an operate winding in electromechanical relay and a bias winding in electromechanical relay.  
The bias is basically describing the differential spill current divided by the mean through current.  
So, bias protection, high impedance protection limits for spill current to a value less than the relay setting, so, the relay will not operate because the current has been reduced to a value below the operating setting relay.  
We can often think in terms of voltage as well, so, what we've done by the high impedance scheme will reduce the operating voltage to a value less than the relay voltage the setting voltage.  
So, under the worst case external fault, we ensure the worst case voltage across the relay and the stabilising resistance is below the operating voltage of the relay system.  
Low impedance protection provides no such limits on spill but artificially raises setting of a relay, so, what we do is we have a bias characteristic and what we do, the higher the through current, the higher the potential spill, and effectively the greater increase in the setting required.  
The increase in setting is normally based on a percentage of the through current, and the protection is commonly referred to as a percentage bias differential protection scheme.  
The advantages of current differential protection are no voltage transformers required.  
I think this is less important, to be honest.  
We normally have voltage transformers available, certainly a higher voltage, we may not have them at 11 kilovolts.  
And current differential protection does not require voltage transformers because it only operates using current.  
It's ideal for multi terminal feeders, so, of course, two terminal or 3 terminal, 4 terminal, 5 terminal, however many terminals.  
You can detect high resistance faults.  
It's immune to be impacted power swings which can cause serious problems for distance protection.  
During your distance protection lectures you've learnt about the problems caused by power swings and how they may cause maloperation of protection.  
A current differential protection has a consistent operating speed, so, there's the same operating speed irrespective of where it is, where the fault is located on the line.  
You can apply them to series compensated lines.  
They're simple to set with no coordination problems, so, it's very, very easy to use differential protection.  
For challenges generally about how do you communicate the information from one line end to the second line end.  
I'm now going to talk about methods that we use.  
So, you have differential protection using pilot wires, these were the first schemes and first began to be used, I guess 1930s, so, perhaps over 80 years ago.  
And differential potential was classically implemented with metallic pilot wires.  
A pilot wire is not a three phase system, is deliberately, effectively, a single, well, two wires, so, it's designed to be simple.  
So, what you have to do is you have to summate the signals.  
During our exercises, during our whiteboard exercise, we will begin to look at methods we can summate the signals.  
If we just added the signals from each phase equally, we would get effectively a positive sequence value and it wouldn't work, a zero sequence value, and it wouldn't work for all fault types.  
So what we do is we add the signals in a nonlinear way, so it works for single phase faults or face to face faults or three phase fault.  
So, the pilot, the communication pilot referred to as a metallic pilot is a single phase replica of the primary current.  
The maximum length of that pilot is approximately 30 kilometres, we can't go beyond that because for capacitance effects of the pilot become significant.  
This system is very susceptible to electrical interference, so, great care is required when using metallic pilots.  
So, when you look at different communication options, we, of course, we started with metallic pilots, then in 1960s we began to use electronics and we would convert our 50 or 60 Hertz quantities into a frequency response.  
Effectively, a high frequency signal.  
So what happens in that diagram, the middle diagram there, when the voltage is high, we communicate a high frequency.  
When the voltage is low, we communicate a low frequency.  
And then we recreate, we convert that frequency modulated signal back into a current signal.  
That technique was very popular in 1960s, 1970s, 1980s.  
But by the 1990s we'd moved into the digital world and we began to use digital communication techniques.  
So what we did we took the analogue signal, we converted it into a digital signal, we passed it into a microprocessor and we communicated it by a digital communication interface.  
Again, we will discuss in great detail how the digital communication systems operate.  
So, a lot of effort and time we're going to describing how to use a fibre optic current differential protection scheme.  
Thank you very much.  
I hope you enjoyed the talk about differential protection.  
So, I look forward to more talks at a more detailed level about the behaviour of differential protection applied to feeders.  
  
  
  
# 3.2 EPSE Differential Protection Tutorial  
-- LECTURER:  
Okay, welcome back.  
So I'm returning to the solutions of the tutorial problems for the Protection module.  
I'm now on question two, which is about high impedance differential protection that's used to provide earth-fault protection for generator stator winding.  
So it is designed for only earth-fault protection of that generator stator winding.  
This is very commonly used because the vast majority of faults that could occur within a generator are earth-faults.  
Cause if you think about the construction of a generator, it is unlikely you'll get a phase-fault within a generator.  
It's not impossible but it's unlikely.  
So this particular generator, as described in question two, is rated at 5MVA, 3.3 kv, and has a sub-transient reactance of j0.1 per unit.  
So 0.1 per unit, based on the machine rating.  
The stator winding is earthed via a single phase grounding or earthing transformer, which has got a...  
So it goes from 1.9 kv, in other words 3.3 kv divided by root three, so the phase-to-neutral voltage.  
And that's referred to 240 volts.  
So effectively on the 240 volts side, we connect a secondary burden resistor, of 0.05 ohms.  
This is then referred to the 3.3 kv side, where it now has a high impedance.  
So I'm going to start by describing the types of faults you could get, and then we're going to discuss what might happen.  
If I look at the diagram, we've got the generator, and of course this three-phase system.  
So those are the three phases.  
And this is rated at 5MVA.  
I just find when you're doing a problem, it's better to draw a picture.  
Most people are better at looking at diagrams cause it tends to help them understand.  
So this remember is the line-to-line voltage of 3.3 kv, the maximum output power, so the rate in output power is 5MVA.  
And the sub transient resistance, impedance, in fact reactance, the sub-transient reactance, is j0.1 per unit.  
And then we're going to ground it, through a transformer, as mentioned.  
So, basically this is 240 volts on this side, and this side will be 1.9 kv which is effective of the 3.3 kv, of the winding divided by root three.  
And when we connect a resistor on here, that is then referred to the secondary, and will limit the fault current.  
So it limits the fault current, that flows.  
What we're trying to think about, when you get a ground fault on this winding, say we got a fault here, that's flowing to ground, we're trying to limit the current that's flowing into the generator, under fault conditions to try and limit the damage.  
So the resistance on the 240 volt side, so the LV side of the grounding, is equal to 0.05 ohms.  
Which when we refer this to the 1.9 kv side, so, effective of the 3.3 kv side, is 0.05, multiplied by 1.9, divided by 0.24, all squared, which gives an answer, of 3.13 ohms.  
So, you can see that really this impedance, this looks like a resistor of 3.3 ohms.  
So, this is the earthing, or grounding resistor.  
In English we tend to use the term earthing, in America the term grounding is used, and I tend to oscillate between them.  
So, this is the earthing resistor which is equivalent to 3.3 ohms.  
Now let's look at the rated output of this generator.  
Then what we're going to get is I-rated, is equal to 5MVA, divided by root three, times 3.3 kv, which works out at 0.875 kA.  
So 875 amps flowing.  
Now if we begin to think of what happens.  
So if we think about a terminal fault.  
So this is a fault across the terminals of a machine, so effectively this location.  
And let's start by thinking about a three-phase fault.  
So this is across the terminals and it's possible to have a terminal fault that's three phases there.  
What it would normally be, is somebody's left the earth clamps on.  
So when they'd be doing maintenance, they would have grounded the system, and they've left the connections on accidentally.  
So if we've got a terminal three-phase fault, what do we get?  
Then I-primary, on the phase three phase, so the primary current is I-rated, divided by Xd".  
That's the short way of doing it.  
And it's something you might remember.  
If you don't remember it, there's a longer way of doing it, which I'll do in a moment.  
This gives you an answer of 8.75 kA.  
because of course, it's this value divided by 0.1.  
So we take that 0.1 value, just take 0.875 divided by 0.1.  
In addition, I-primary three phase, is equal to kv line-to-line, divided by root three, all divided by X per unit, times affective of the Z of the base, so the base impedance value.  
And the Z of the base, is equal to kv, line-to-line squared, divided by MVA.  
So of course if we start substitution in this equation, we find the Ip three phase, is equal to kv line-to-line.  
I'm going to move the root three below, times X per unit, times kv line-to-line squared, divided by MVA.  
So at that point, I can cancel this one against that value.  
And at that point, I reduce this to MVA, divided by root three, times X per unit, times kv line-to-line.  
So when we start putting numbers into this, for this example, so in this particular example, that Z base would be equal to 3.3 squared, divided by five, which gives an answer of 2.178.  
And when we put the values into this equation, we find we've got five, divided by, root three, times 0.1, times 3.3.  
And surprise, surprise, we of course get the same answer again.  
So we get the 8.75 kA.  
So this is a three-phase-fault and I've sort of done it two slightly different ways.  
This is really the short way of doing it if you remember that.  
So, it's to remember that if you put a, effectively, the sub-transient reactance of a generator, or the leakage reactance of a system, you take the rated current divided by the sub-transient reactance of leaked reactance term to get the fault current.  
I'm also going to do this, explain this a slightly different way just to give you completeness of understanding.  
So in this case, I-primary three...  
Let me just quickly change my...  
So I-primary three-phase, is equal to, kv line-to-line root three, X per unit times X base.  
I'll show you why I'm doing this in a minute this particular way, because I'm going to then expand it for the case of a phase-to-phase fault, and a single-phase fault.  
So this will of course, give the same answer 3.3 root three, j0.1 multiplied by 2.178, and I get this answer which of course is exactly the same as before, 8.75 kA.  
So that's for three-phase current.  
Now what I want you to think about is the phase-to-phase terminal fault.  
So this is where instead of having the three-phase fault up here, I've actually connected a phase-to-phase fault.  
So what I've done now, is I've taken this value, and I've connected a phase-to-phase fault across it.  
So, effectively marked down where I've shown it here if I said that was the a, b, c, and I've put the fault across for b to c phases on the terminals.  
And then I-primary, phase-to-phase, is equal to, kv line-to-line, divided by twice Xd", but in ohmic values this one.  
So this is going to be, OK I'm going to multiply by Xd" for the per unit value by the base, so we must have the ...  
previously I described it as Z-base, so that'll be complete.  
So I'm going to call that Z-base.  
Now I'm going to put the numbers in, and I get 3.3, divided by two times j0.1, times 2.178, and that is equal to 7.57 kA.  
So for the phase-to-phase fault, we get 7.57 kA.  
And for a three-phase fault, we get 8.75 kA.  
What I'm now going to do, is think again and think of what happens if I put a phase-to-earth-fault.  
So I'm going to change this again, and I'm going to connect effectively a fault now, to earth.  
So in this case, I'm going to pick an a-phase-to-earth-fault, and I'm going to look at the behaviour.  
I need this later in the question to answer it, but it's useful just to derive it here to begin to understand, how the grounding resistor will change the current.  
So of course if I put a fault here, obviously I've left that in there, but that really is gone.  
We do not have a fault there.  
So what we've got is a phase-to-earth fault at that location, and the current flow is effectively through here, and back around.  
So it's limited by this earthing resistor.  
This is done deliberately because the vast majority of faults within the winding, are our single phase-to-earth-faults.  
What we're trying to is limit the damage caused by a fault.  
So again, I-primary phase-to-earth, is equal to kv line-to-line divided by root three, all divided by R in the neutral plus j, times the Xd", multiplied by Z-base.  
So think about where that equation comes from.  
Same structure but this is the dominant one.  
This is the grounding resistor.  
And if I now begin to put the numbers in, I get 3.3, divided by root three, divided by 3.13, plus j times 0.1, times 2.178.  
And this gives an answer, when I put the numbers in, of 0.606 kA.  
This is interesting because now we've got an earth-fault current of 606 amps.  
While originally the rated current of the machine, is 875 amps.  
So we've limited the fault current, so we're going to cause less damage to the machine, to the generator, if a fault occurs.  
Interestingly, if I made the grounding resistance, if just for completeness, if Rn was equal to zero, so if I got a perfect grounding system, and I was grounding for zero ohms, then this value of current, I-phase, sorry, I-primary phase-to-earth, so the I-primary phase-to-earth, would be equal to and surprise, surprise, exactly the same as before 8.75 kA.  
So we get the same answer.  
Now I'm going to sort of redraw the primary diagram, and then draw the connections of the current transformers and the protection relay.  
In this case remember, I'm assuming a high impedance protection relay, or I'm beginning to utilise something called a stabilising resistor.  
The stabilising resistor as you will see, is to ensure that the relay remains stable, on the worst case, external fault.  
So, the relay now is a voltage operated relay.  
So it operates when the voltage across the relay, and the stabilising resistor is greater than a pre-set value.  
We're trying to determine the pre-set value that ensures it remains stable on the highest current external fault.  
But of course, it can still detect an internal fault.  
And you'll begin to see some of the challenges.  
Actually high impedance differential protection has been used for many years.  
It was first used in the 1930s.  
And a lot of work was undertaken in Newcastle, at what was then Huero, which is now a part of the Siemens group.  
So, they almost were the leaders of some of the high impedance differential protection, certainly within Britain, so in the British system.  
So when we look at the system, I'm going to first of all draw the primary system again.  
This is a generator I'm just making it a little bit shorter, so you don't see quite so cause I'm what I'm interested in is really the connections of the current transformers, and the connections to the relay.  
And of course, this is the connection, to the grounding resistor.  
I'm sort of drawing it in a special way because I know it's going to to take me space to draw the network diagram.  
And then what I'm going to do is put a current transformer in here.  
In a protection, current transformers are one of the most important devices actually.  
They've been used for probably now over 100 years.  
And although now there are alternatives like optical fibre current transformers, conventional current transformers dominate the market.  
And I'm guessing 99% or maybe even 99.9% of current sensors used on transmission, distribution, generators, industrial systems, at voltage levels above a few kv are using current transformers.  
So what I'm going to to do is connect these current transformers in series, sorry in parallel, I got that wrong, I'm going to connect the current transformers in parallel.  
Because the thing I'm interested in is earth-fault protection.  
So all I'm trying to achieve is earth-fault protection.  
Reason I'm only really interested in earth-fault protection, is because the vast majority of faults on the generators are earth-faults.  
And this is an inexpensive system.  
So I'm connecting them here, then I connect them that way.  
If you want to be sure you've connected it correctly, what you could try to do, is you could try and put an external fault on here and check that the current flows are consistent.  
I'll show you in a minute what I mean by that.  
So then connect it across phase, so we have the relay, which of course has affected the impedance.  
And then we put in something called a stabilising resistor.  
So we're representing the relay as a resistor, I'm just going to call that R of the relay, and I'm going to call this R of the stabilising resistor.  
And this is a special resistor you add, in this high impedance, you sometimes see it called Hi-Z Diff Scheme.  
Very, very popular around the world.  
It's arguably, differential protection is one of the best forms of protection.  
So this point, let's just think a little bit.  
What happens if we put a phase-to-phase fault.  
If we put a phase-to-phase fault here, and what happens is we could have said that current flows in this direction, and then returns in this direction for a phase-to-phase fault.  
When we get that situation, this creates a voltage, in that direction, and this creates a voltage in this direction.  
Of course, in the same way, remember this is the secondary of the CT side.  
This is driving a current in that direction.  
And this is driving a current in this direction.  
So, when you look at that scenario, assuming it's balanced, there's no saturation at that point of view.  
There's no current in the relay.  
This is a high impedance, remember, so there's no current flowing through that relay.  
So it's a Hi-Z.  
So if we think about this, for external faults, and I want you to convince yourself this is true.  
So for external faults, let's just first start by thinking that all the CT's, are operating in a linear region.  
What does that mean?  
They're operating in the linear region.  
Remember with a current transformer, we have the classical, hysteresis characteristic.  
So when we first switch on a current transformer, okay, if we're driving it to a high current, it goes up like that, and then it goes back down like this, and it goes back like this.  
So it's operating, and effectively, it's going round that hysteresis loop.  
And this is often what we call the BH.  
Where this H is proportional to the excitation current, and B is proportional to the voltage.  
So it's going around that loop 50 times per cycle.  
Normally when in the linear region, it basically means we're operating here.  
So it's just within this bound here, or maybe going slightly higher.  
But it's below the Knee Point Voltage of the CT.  
So it's going round and round that loop in linear, and it's not saturating, so that the excitation current, is staying small.  
If we get an internal fault, what would tend to happen, we will go deep into saturation, and we get a huge volume of excitation current.  
So this is the problem with excitation.  
So, that's about the linear region.  
So in the linear region, if we have a three-phase fault at the terminals, so this is external remember, three-phase fault Obviously the current in the neutral, the neutral CT is zero, three phase fault, balances to zero current.  
So IN, is equal to zero, and I-relay, is equal to IA secondary.  
And these are the vectors plus IB secondary, plus IC secondary.  
And of course because of the, 120 degree phase shift in the EMFs, so effectively you've got EMF equals E angle zero for the a-phase, E angle minus 120 degrees for the b-phase, E angle minus 240 degrees for the c-phase.  
This all sums up to zero.  
So the classical three phase system.  
So there's no current in the relay.  
So for this external fault, three-phase fault no current in the relay.  
So if we put a phase-to-phase fault as I explained before, effectively I-relay now, is equal to, I, I'm going to just use a term IB phase on the secondary minus V is a vector of course, minus I, the c phase which is minus IB, as shown on that diagram.  
So, of course, this is also zero.  
If we think of a phase-to-earth-fault, I-relay, if I assume it's on the a-phase in this case, so let's now switch to the a-phase current, this is going to be rather hard to draw.  
So I'm going to, of course, now I would have changed all these currents slightly.  
So I'll get rid of these, get rid of this one.  
I suppose I should get rid of that.  
I'm just going to redraw this at this point.  
So at that point now I'm going to put an a-phase fault to ground, so I'm connecting that to ground.  
Just for clarity, I'm just going to show that at a slightly different angle so, at the terminal, I'm just going to show so it's a fault, so the current is now flowing this route.  
So of course, let's think about this.  
So it's doing that.  
So this one when we think about this, CT is driving, it's creating a voltage there, which is driving a current here, which is then flowing down through here, which of course this one, the voltage is in that direction, which means that the current flow is that.  
So actually, when you analyse that system, there's no current flowing through the relay because current effectively flows around that loop like that.  
So effectively the I-relay is equal to IA secondary, minus I-neutral secondary, which again is equal to zero.  
So the current in the neutral, cancels the current in the a-phase.  
So now we're going to begin to think, about what happens, when a line CT, is fully saturated?  
And when we think about fully saturated, it means that only this hysteresis loop, we've forced it to a deep saturation.  
And actually what we've almost said now, the current transformer we're using, is going to be looking like that.  
So that's fair.  
Let me redraw that a little bit to make it just slightly more consistent.  
So I'm going to assume, the CT is there, then what I'm going do is plot across it, the magnetising resistance.  
And what I'm going do now, is assume the magnetising resistance is fully saturated.  
So what it means, is there's a perfect short circuit across it.  
This is obviously a worst case scenario, but for a high impedance scheme, you start by assuming the worst case scenario.  
And the worst case scenario, is for deep saturation, is for a short circuit across the secondary of the CT.  
I'm going to start by drawing, a phase-to-phase fault.  
I'm going to put a fault here, at that point.  
So effectively I've put a fault across this point.  
So from the b to the c.  
So effectively current flows here, and comes back here, on that position.  
And I'm now going to assume that this CT is fully saturated, which means that I can put a short circuit across the CT.  
But it's magnetising branch, means that all the current flowing out of the CT, is not leaving the CT.  
It's within the magnetising circuit.  
And of course, what I want to do now, is I'm going to consider this phase-to-phase fault, and I'm going to assume a Hi-Z relay.  
And the CT ratio, is equal 1000:5 So the I-fault current on the secondary, for a phase-to-phase fault, as we calculated before is 7.57 kA, divided by 1000:5.  
And that is equal, to approximately 7.6 times I-nominal, where, I-nominal equals five amps.  
On a protection system, the two nominal ratings of the current transformers, are either one amp secondaries, or five amp secondaries.  
As a gross generalisation, it's not always true, but on transmission systems, most of the networks use one amp secondaries, while on distribution networks, most of the networks use five amp secondaries.  
Although interestingly, many years ago, there was a five amp CT used on the system near London.  
And, they had to change a relay because a protection relay was failed.  
So that point they changed it, and they incorrectly changed it for protection relay, which normally had an operating current of one amp.  
So they put a one amp relay, instead of a five amp relay.  
It's a bit like with a fuse, so instead of putting a five amp fuse, they put a one amp fuse in the system.  
In fact, this was near London and the system coped for about one year.  
And then on one particular day when the network was heavily loaded, this protection relay falsely tripped, and disconnected half of London, from the electricity network of Britain.  
And of course, the economic cost of that failure, was very, very significant.  
After that, every protection relay on the British system was checked to determine that there were no other stupid mistakes.  
Regrettably, we all make mistakes.  
So when I put those numbers in, that translates to a current of 38 amps.  
So the voltage across the relay, when we begin to look at this network, I'm going to now expand it out.  
So what we've got now, we've got this CT from the b-phase, which is connected through a resistor, to the relay.  
I'm just going to to show the ...  
And with the stabilising resistor.  
I'm just drawing it in a slightly different way.  
And then what we've also got, is the second CT, which is now fully saturated.  
So I've put a short circuit across this, and this is also there, we've got the connection.  
And then we connect those to that, and then that to that, And that really is how the connection details would be.  
So I've individually connected each individual CT to the relay circuit.  
And this would be the normal procedure we would do.  
When you begin to look at that diagram, of course what begins to matter is, this is a stabilising resistor, this is the resistance of the relay, and these are the lead and CT resistances.  
So, we describe...  
let me just expand that a little bit.  
So, our value of R there, is equal to resistance of the CT, plus the resistance of what is basically the leads.  
Actually interestingly the leads are always operated as a twisted pair.  
So we twist two leads together and this is like the circular impedance of the leads.  
In this particular question, the CT resistance was 0.2 ohms, and the lead resistance was 0.8 ohms.  
So of course, deliberately to make the problem very easy, that is one ohm.  
So it's a one ohm resistor.  
So now, when we begin to look at this, this protection system is voltage operated.  
So to operate that relay, we need a voltage greater than the setting.  
So, this is the voltage of a relay plus for stabilising resistor.  
In this particular case, the operating voltage of a relay is 30 volts.  
So the V-operate relay, is equal to 30 volts.  
And actually this particular relay, operates at 30 volts, at 30 mA.  
So, it operates it requires 30 mA to operate, because actually, it's impedance of the relay.  
So, the R of the relay, is equal to 1000 ohms.  
So, the resistance of a relay is 1000 ohms.  
So now what we want to calculate, is what is the voltage across the relay and the stabilising resistor.  
So the voltage across, so it's across the relay, and the R-stab.  
It's going to be equal, this is producing the maximum current through here, and of course if that's flowing through here, this is a high impedance of 1000 ohms, so of course the current effectively flows through here, and back through here.  
And what I'm interested in, then, and this is a short circuit, so the voltage across the relay and the stabilising resistor, is this value of current, which is 38 amps.  
So remember, on the primary, we had a current of 7.57 kA.  
On the secondary, we have a current now of 38 amps.  
So this is 38 amps, multiplied by R of the CT, plus R of the leads, and as I mentioned they'd come to one ohm in the question.  
So we've one ohm.  
So this gives a value of 38 volts So 38 volts.  
Right, at this point you can see that this voltage would operate the relay because the relay only required 30 volts to operate, we have 38 volts, therefore the protection would falsely operate.  
We cannot allow that to happen.  
But this protection is designed to protect the generator.  
It is not designed to protect the system and to trip off the generator.  
We want the generator be left connected.  
So, because what we would normally expect is there's other protection downstream of the generator into a network which will clear the fault.  
If you think about that situation, if National Grid has a phase-to-phase short circuit fault on the network, you don't expect the generator at Sizewell B to disconnect due to a problem.  
The National Grid System is protecting the transmission lines, and the generator protection that belongs to the owner of the generator, is protecting the generator such as Sizewell.  
Right, so if we look at this again, so the relay, the relay, as I mentioned is 1000 ohms.  
So we want to drop, effectively greater than 18 volts.  
Well effectively we want to drop the 18 volts, across R-stab.  
So the value of R-stab we will choose, is 18, divided by 30 times 1000, to get an ohmic value, that gives us an answer of 267 ohms.  
So we need an R-stabilizing resistor of 267 ohms.  
So if we connected a 267 ohms resistor in that location, and the real impedance is one kilo ohm, then that relay will not operate for that phase-to-phase fault.  
Now of course, I want to consider what happens on a three-phase fault.  
This is now a little more complicated, because on a three-phase fault, we have the behaviour of all three phases.  
What I'm going to to start with now, is consider a three-phase fault.  
And again, this high impedance relay.  
So my three-phase fault, is I've got a fault here, fault here, and a fault here.  
So it's a balanced three-phase fault across all phases.  
Normally, as I mentioned before, a three-phase fault would have been caused by somebody leaving the earth clamps on.  
So they've literally earthed it down, they've re-energized the system with the earth clamps on.  
That's probably the main cause of three-phase faults.  
And I'm going to assume again that one CT is saturated.  
So when I look at the primary, so IA primary, is equal to 8.75 angle zero degrees kA, as we derived before.  
So of course what we've done, and IB primary, is equal 8.75 angle minus 120 degrees kA.  
And, IC primary, is equal to 8.75 angle minus 240 degrees kA.  
So it's a balanced three-phase set.  
So of course the current in the neutral in that case is I-neutral.  
So I-neutral, is equal to zero.  
So now the voltage across the relay, and the stabilising resistor.  
And again, it's the same as before, again I'm going to draw it as before.  
This is rather hard to draw.  
So when we look at this voltage, what do we get?  
This is where the voltage.  
So what do we get?  
So the voltage here, is going to be the, in this case the IA secondary, IB secondary, and then that flows back.  
Remember this is high impedance.  
So this is this Hi-Z.  
So the current then flows back into here, and then that loop.  
So the voltage across the relay and the stabilising resistor, is equal to, 8.75 angle zero degrees plus...  
Okay I'm just going to do it.  
Where previously which was, I've actually drawn just to make it slightly more clear.  
I'm actually going to slightly change this.  
And I'm going to remove the...  
I'm going to save it.  
It's not that's CT.  
Actually, can I start again, let me just start from this point.  
STUDENT:  
Start from the scratch.  
I'm just, okay I'm going to move that, STUDENT:  
(mumbles) Right, and I'm going to put my...  
It's only my example is solved for this one.  
STUDENT:  
Sure.  
And always I have to calculate what the angles are.  
So I'm just going to put the short, is here.  
(crosstalk) Okay.  
I'm going to start this again, because I made a slight mistake in terms of my example, although it would have given the same answer, but it would have been more complex.  
And what I'm going to do, is assume the a-phase, CT is fully saturated.  
So you can see in this diagram, I've put a short circuit across this path.  
And now what I'm going to do, is draw this out.  
So I'm going to draw this in more detail, to explain this connection.  
So this is the a-phase CT.  
I'm assuming its got a short circuit across it.  
And then I've got the b-phase CT.  
And then I've got the c-phase CT.  
And then, the relays in this location, the stabilising resistor is here.  
So that's the R-stab, And that's the R of the relay, then I'm going to connect those to here, actually it would have been better, let me not just draw quite like that.  
Let me just draw it that way.  
And then I'm going to draw this that way.  
And what I want to emphasise, is the current transformers, but it's obviously electrically the same.  
But what I want to emphasise is the current transformers are individually connected by the twisted pairs to the relay circuit.  
And now of course, because of a saturation what I get is the current from the b-phase.  
So, IB on the secondary, I get IC on the secondary, which then flows back into the a-phase circuits.  
So the current in there is IB secondary, plus IC secondary.  
So, this point what I'm going to say is the voltage across the relay...  
So the voltage across the relay and the R-stab, the stabilising resistor, is equal to, 8.75 angle minus 120 degrees, plus 8.75 angle minus 240 degrees, all multiplied, by RCT plus R-leads, and remember these above the c-phase CT.  
So it's of the a-phase CT.  
The a-phase CT, which is one ohm.  
And now I need to think, well what does this mean?  
Okay one way is to draw it vectorially.  
So of course what we would normally have done, is we draw our three phase set.  
And of course we've got normally IA, IB, IC, and of course with that rotation.  
I'm not showing the three phase balance set.  
In this particular case, because of the saturation of the current transformer, the a-phase disappears.  
So at this point we've got the vector IA, plus the vector IB, and what you actually get is this value here.  
So effective in this case, IB plus IC, is equal to minus IA if it was there.  
So from a primary side, actually those on the primary side.  
The one thing I'd forgotten to do in this example, is divide by the CT ratio.  
That should all be divided by the CT ratio.  
So of course, so from the primary side, on the primary, but of course, we don't really have a primary.  
So we want to think of a primary, but we are getting a value here, of 8.75 angle minus 180 degrees, of course, divided by the CT ratio.  
And that of course is multiplied by 1.0.  
So when I look at those values, what we get is 8.75, times I-nominal.  
So in this case I've got 8.75 I-nominal, which is equal to 43.7 volts.  
So we get a voltage of 43.7 volts.  
As I mentioned earlier, that the operating voltage of the relay, is equal to 30 volts.  
So I need to drop, 13.7 volts across R-stab.  
And I mentioned earlier that this relay operates at 30 mA, which means that the resistance of the relay, is equal to 1000 ohms.  
So therefore, the R-stab, must be equal to, 13.7, it's actually 13.75 divided by 30, multiplied by 1000, is equal to 458 ohms.  
So that's 458 ohms as compared to before, so for a phase-to-phase fault, we calculated R-stab, was 267 ohms, but now for a three-phase fault, to ensure it doesn't falsely operate on an external fault, we need 458 ohms.  
So we require 458 ohms.  
That's a value we require.  
So we require R-stabilizing resistor is 458 ohms.  
Right, so what I described before is how you ensure that the protection relay that's protecting the generator stator winding for earth-faults, remain stable for all possible external faults.  
So for a three-phase fault, a phase-to-phase fault, external on the terminals.  
So for example on the line the generators connected to.  
But also of course, now what we're interested in is, will the protection protect the generator from an earth-fault?  
We already mentioned that we're limiting the fault current for earth-faults by putting a earthing, a grounding resistor into a system.  
So let's begin to calculate, what percentage of the stator of winding, we can protect for using this protection.  
So the current that flows, so we're going to look at initially that phase-to-earth-faults, on the generator stator.  
If the fault is located at the terminals of the generator, but within the protected zone, so if we start by setting a fault at the terminals, but within the protected zone, and it's a phase-to-earth-fault.  
So a phase-to-earth-fault, at the terminals, within the protected zone, which means it's within the current transformer, the current transformer system.  
So it's on the stator winding.  
We calculated that IC..., a current that of flows in the CT and the neutral, is going to be equal to this 607 amps, divided by the CT ratio.  
So the primary current of an earth-fault at the terminals of the generator, was 607 amps divided by the CT ratio.  
So we get an answer of 0.607.  
I should then put 0.607.  
I'm going to describe it as 607.  
No I'm not I'm going to change my decision and do it slightly different.  
I'm going to put it as 0.607, times I-nominal, where I-nominal remember is five amps, and that translates to 3.03 amps.  
So this translates to three amps on the secondary.  
I'm going to quickly draw the...  
STUDENT:  
Your 607 hasn't turned up.  
TUTOR:  
Okay.  
STUDENT:  
Oh, I know.  
TUTOR:  
Okay, let me...  
STUDENT:  
Right.  
Right.  
So when we looking at this system, what we've got is we've got the generator, and we've got the CT's, and we've got the relay, and we got the stabilising resistor, then what we're going to do is put a fault here.  
So we're going to think of an a-to-earth-fault, literally on the terminals of a generator, but within the protected zone.  
So of course, if we think about the current, that creates a current here, which flows into here.  
This is the ground, so it flows back round that loop.  
From the secondary side, this creates a voltage on the CT, which then drives the current through that way.  
So the current now, there's no current in any of these, so consequently it's going to flow, it's going to create a voltage across the relay.  
So the zero amps in any of these, so we're assuming, in fact, the question mentioned that we assume the generator, there's no feed for the zero sequence from the power network.  
So the fault is not sourced from the power network, the fault is only sourced from the generator.  
So what we'd actually assumed, is we'd connected it through a delta-y transformer to get rid of the zero sequence.  
And by using this delta-y transformer, we get rid of the zero sequence.  
But what I'm really saying is there's no current from the network side, everything's from the generator.  
So now we begin to think about the current, required to operate the relay.  
So how much current is required to operate the relay?  
So the current required to operate the relay.  
And now of course, what we begin to think, there's no current actually flowing around this network.  
So it's all about voltage.  
So basically, on the system, we need a voltage here, and if there's no current flowing, this is basically very small.  
So if we think about a voltage-operated relay, if we think about this as a very high impedance, and what it means is if there's no current in here, and what we have is we have a voltage here, voltage is the same across here, voltage is the same across here.  
So the voltage of all points in this network are the same.  
What I'm now interested in, of course, is well what does the magnetising branches of all the CT's do?  
So I've assumed, that this CT has got its magnetising branch, This CT has got its magnetising branch, This CT has got it's magnetising branch.  
And of course, all those magnetising branches take an excitation current, which depends on the voltage.  
If I draw this slightly differently, you can see that what I'm really doing now representing the secondary, we've got an AC source, which is now got the magnetising branch of the first CT, it then is connected to the relay and the stabilising resistor, and then that is connected to the next magnetising branch of what is the c-phase CT.  
And then it's connected to the magnetising branch of the b-phase CT, and then the a-phase CT.  
So what we've got is four magnetising branches.  
So we've got this excitation current, so each of these has got an excitation current, so the I-operate, is equal to I-relay, and I mentioned that to operate the relay required 30 mA, plus four CT's in parallel, I made the assumption that all the CT's are identical, if the CTS are different you have to take that into consideration.  
So, you got four times the excitation current.  
And the excitation current comes from your graph, of the BH curve of the CT.  
So, what we would have done, is we would have plotted the BH curve of the CT, which I think is described as the voltage of the terminal of the CT, versus the excitation current.  
And remember on the numbers you are given in the question, at Vs is equal to 40 volts, I-excitation, was equal to 60 mA.  
The voltage on the terminals, I should have used Vt there.  
So let me just put Vt, and this one is now at 50 volts.  
Of course, you could draw the diagram but obviously under exam conditions, I would have just done a very simple approximation.  
So actually what I'm going to to say now, is at...  
The voltage we had remember, we calculated early.  
The voltage to operate the relay is 43.7 volts.  
That's for the voltage to operate the relay.  
And for Vt equals 43.7 volts, I-excitation is approximately equal.  
I'm assuming a linear interpolation now, is 60 mA, plus (coughs) 3.75 divided by 10 multiplied by the excitation current difference of 30.  
So I've used a linear interpolation technique, and I come up with an answer.  
The excitation current is 71 mA.  
So I've got 71 mA, is the current to operate as the excitation current.  
This current there, is 71 mA So, if I put all those together, what I get, is a current now a 314 mA So, the current that needs to be created by this CT, is 314 mA.  
And of course, this depends on where I put my fault, because as I move my fault closer to the neutral point, the current will reduce.  
So, for a terminal fault you got 3.03 amps.  
The operating voltage is 314 amps.  
So the percentage of the winding protected, using these numbers together, is equal to 100% minus 0.314, divided by 3.03, multiplied by 100%.  
And you get an answer, of 89.6%.  
So effectively, we're almost protecting 90% of the generator.  
I'm just going to check this.  
Because just to check that my calculations are right, and partly to help you understand it.  
If we consider a fault, at 11% from the neutral, so it's 11% from the neutral.  
ICT in the neutral, is equal to 0.11 multiplied by 3.3 kv divided by root three, divided by 3.14 angle four degrees.  
Remember I'm using this from the value we calculated earlier.  
I put those numbers in, and I get an answer, of, and that's divided by the CT ratio as well, which I'd forgotten to put in, so divided by the CT ratio, and I get an answer of 333 mA.  
So for a fault at 11%, so effectively 89% for the winding.  
Convert 11% from the neutral, we get a fault current of 333 mA, which is larger than the 314 mA.  
So effectively operate.  
So this is greater than 314 mA to operate, which is what you'd expect.  
And then of course for a fault at 10%, so the ICT in the neutral, same as before, but now in this case worked out at 303 mA so it does not operate.  
So the relay does not operate.  
So you can see that this protection system, is protecting almost 90% of the winding.  
But for a fault very close to the neutral, there's not enough current to drive the system, and it will not detect the fault.  
This is a commonly known technique.  
This technique cannot protect 100% of the winding.  
If you want to protect 100% of a winding, you often will apply very complex techniques, which perhaps use a harmonics created by a generator.  
But these are only applied to the most important machines.  
So maybe if you've got a 1.6 GVA large generator for a nuclear station, you will put something called 100% stator earth-fault protection.  
This particular protection technique is giving you 80 or 90% stator earth-fault protection.  
Normally we anticipate this technique to give about 80 or 90% protection.  
But it does not protect 100% of a winding.  
But of course when you begin to think about it, what is the chance of getting a fault, near the neutral point.  
It's more likely to get a fault near the line terminals, because they're more likely to be affected by maybe a lightning activity on the transmission line, which causes a flashover.  
Although it is a very complex phenomena, because if you do have lightning, it tends to propagate down the windings, and the flashover point can be within the windings.  
It may not be at the terminals.  
So thank you very much.  
I hope you've learned a little bit more about stator earth-fault protection using high impedance differential protection.  
Thank you.  
  
  
  
# 4.1 Principle of the operation  
--LECTURER:  
Hello.  
My name is Vladimir Terzija, I'm the professor at the University of Manchester, and welcome to master power system protection module.  
I will be teaching you sections 5, 6 & 7, and in these sections you will be in a position to learn more about principles of operation of distant protection which in my personal opinion is one of the most complicated but also sophisticated protection functions and protection types used for protection of different elements of power system.  
Furthermore, I will go to something what is today particularly important, application of modern digital relays or numerical protection.  
This topic is quite important because it will introduce us to another topic, wide area monitoring protection and control which is today becoming more and more popular and it is enabled by high technology, sensors and ICT, information and communication technology.  
In this context I'll also address something what is related to aspects of application of communication protocols in communication infrastructure.  
And last but not least, I'll be focused on motor protection which is quite exciting.  
So, let us move now to the first section, section number five, distant protection.  
You have been already introduced different types of protection.  
Now, we will start studying distance protection.  
These different types which you went through where, for example, over current protection, differential protection.  
So, in this lecture we will be focusing on questions like, why distance protection?  
We will be discussing functionality and technical details related to requirements necessary for an optimal operation of distance protection.  
We will be focused also on different applications, furthermore on distance protection schemes.  
And the last but not least, we will address the issues related to fault location.  
Firstly, let me introduce basic principles of distance protection operation.  
Next to this, I will discuss why distant protection is necessary, why protection of modern power systems would be impossible without distance protection.  
You have already learned how for example overcurrent or differential protection operate, this kind of protection functions or types of protection are relatively simple and straight forward, for example, overcurrent protection requires 1 input signal, this is the current.  
Whereas differential protection requires 2 currents or in a three phase system, 3 plus 3, what means 6 currents.  
So, in principle, distance protection is a universal short circuit protection.  
And differently to overcurrent or differential protection the mode of operation of distance protection is based on the measurement and evaluation of short circuit impedance.  
Thanks to its flexibility, it is used for protection in transmission and distribution networks, this is such a fantastic thing to have a protection principle which can protect both transmission and distribution networks.  
Finally, distant protection is faster and more reliable than the classical overcurrent protection, this is very often, very important to ensure that the operation of power system will be stable and as planned and scheduled by those who are running the power system.  
I have mentioned one important point, that the distance protection is more selective, what does it mean?  
Firstly, return it back to a definition of selectivity.  
Selectivity means, if a fault the element, if a fault happens on an element, the protection will disconnect, only the faulty element.  
So, in this context, distant protection has higher level of selectivity compared to the classical overcurrent protection.  
In this slide, I would like to address those issues related to protection selectivity requirements.  
So, as you can see in this slide, two single line diagrams of two different networks are given.  
The one on the top is a typical radial network, used often in distribution networks.  
The one below is the network fed by two generators or two active networks.  
When it comes to protection of the radial networks, just application of overcurrent protection would be sufficient to ensure the full selectivity and selective operational protection.  
But in the second case, in the case of the network fed by two active networks, just using overcurrent protection, a selectivity couldn't be ensured.  
That's why application of time graded directional overcurrent protection is necessary.  
So, the selectivity requirement is satisfied in a way by using time grading of, in the first case, in the case of radial network overcurrent protection.  
But in the second case, in case where direction overcurrent protection is used.  
So, the second network could not be selectively protected by using just overcurrents release, this is the important message.  
So, below in the third graph, below the overcurrent response time versus line length is given.  
Let us analyse protection of the network presented through the upper single line diagram.  
So, you can see that this is a network fed by two generators which are connected to one busbar, and from this busbar follows a transmission line, number one, and probably the rest of the network.  
And we are talking now about the protection of this transmission line which is connecting this busbar and the next transmission line on the right side.  
So, in the first case, for a fault f1, in this case the fault current is 7380 amps, the relay should not operate, why?  
Because the fault is not on the line which is protected.  
The relay should not operate if the fault happens on another transmission line, this is selectivity requirements.  
So, in this case, the current which should be set on this relay, overcurrent relay, must be larger than 7380 amps.  
On the other hand for the fault f2, for example, you see in the diagram below.  
But in the case when one of generators has been disconnected from the grid, for example, because of maintenance reasons, the fault current would be 6640 amps, and in this case relay must operate.  
So, we have two contradictory requirements.  
So, that overcurrent protection cannot be used for protection of this transmission line.  
An alternative solution would be application of differential protection or distant protection.  
Modern transmission and distribution networks are traditionally meshed networks as presented in this slide.  
Such type of networks cannot be selectively protected using, for example, overcurrent or directional overcurrent protection.  
That is why we need other types of protection.  
Principle end by using distance protection a fully selected protection of meshed network could be achieved.  
This is achieved by utilising the principle of operation of distance protection which is based on measurement of impedance to the fault.  
I would like now to more precisely introduce distance protection.  
So distance relays are normally used to protect transmission lines.  
They can be also used for protection of cables and they are traditionally used also for protection of other elements of policy system for example transformers or generators, it depends on the application.  
They measure impedance to the fault as I said.  
What means they are so called fault impedance and the complex R-X diagram is a tool for describing and analysing a distance relay characteristic.  
As I have already introduced, distance protection requires two input variables to measure impedance.  
What means that having both voltages and currents at its inputs it can calculate impedance.  
In this context it is more expensive protection because it requires both the current transformers and voltage transformers.  
From the perspective of operation of distance protection and correct measurement of the impedance to the fault.  
It is critically important that for a given fault and appropriate selection of input variables I mean combination of voltages and currents is used for correct operation of distance protection.  
Let me now introduce two fundamental principles of operation of protection operation of protective relays.  
So the first principle is called underreaching principle.  
So underreaching protection is a form of protection in which the relays at a given terminal do not operate for faults at remote locations on the protected equipment.  
For example look at the transmission network which is now given in this slide we see two transmission lines.  
And let's focus on relay distance, relay RAB.  
So this distance relay is utilising underreaching protection if it is protecting this transmission line up to the certain point.  
For example 80% of this transmission line.  
So it will operate for all faults which can happen up to 80% of this transmission line.  
for other faults this protection will not operate.  
On the other hand there is so called overreaching protection.  
And this is a form of the protection in which the relays at one terminal operates for faults beyond the next terminal.  
So in this case let me now give again example how relay RAB would operate.  
If we would have a fault which is on the right side of busbar B this relay would operate.  
So I have introduced these two principles but let me now discuss one important point which has to do with different types of uncertainties which can occur when determining distance to the fault.  
Instrument transformers means current and voltage transformers are introducing certain level of uncertainty though they are not 100% accurate.  
What means that that what we see on a secondary side doesn't mimic that what is in the primary side of course, we try to have an accurate picture on secondary side.  
However, through manufacturing of different type of instrument transformers.  
We can not ensure 100% accuracy of these devices.  
But you could be having in mind saturation effects which happen on current transformers.  
Next source of uncertainties are transmission line parameters.  
They are probably different from season to season because of changes in transmission line geometry.  
So the uncertainty must be considered when designing distance protection.  
That means that the remote point of each of a distance relay can not be precisely determined.  
And this uncertainty of reach is typically about 5% of the setting.  
As a result of mentioned uncertainties related to instrument transformer and line parameters.  
The concept of distant relay zones is introduced.  
So to avoid mal operation in cases when faults are very close to busbar B now we are talking about distance really installed at bus bar A what means distance real RAB.  
So we will and we can ensure that relay RAB will operate for all faults which belong to zone one but as you can see zone one is not covering the whole transmission line AB exactly because of the issues related to uncertainties introduced by instrument transformers and transmission line parameters.  
That's why we define zone one which is protecting 80% to 90% of the protected line.  
So the rest of the line must also be protected but we introduce another zone which is zone two, which is slowed down by some...  
for example 300 milliseconds and this has to be done because it is going beyond the transmission line AB.  
It is encroaching into transmission BC where the main protection is RBC and full of fault for example F2 the main protection RBC must operate.  
And in this context really RAB when it comes to the operation of zone two must be slowed down not to operate forth for example, forth for F2 but having zone two we ensure that the rest of the transmission line AB what means from 80% or 90% to the 100% will be also protected.  
We also traditionally introduce another zone which is zone three and it is used as a backup protection.  
I would like to point out also when it comes to protection of a transmission line when it comes to distance protection we must have distance really at both sides of transmission line.  
So one really is really looking at one direction and another really is looking at another direction.  
So as you can see we have three zones for relay RAB.  
So we would also have three zones, zone one, two and three which are time related for the protection really is protecting transmission line AB and which is installed on the left side of busbar B.  
As discussed in previous slide each zone of protection has its own operational time.  
Zone one operates instantaneously after zero seconds.  
Zone two for example 300 milliseconds and zone three after for example one second.  
By introducing zones of operation and time delays, the selectivity requirement.  
is satisfied also in meshed networks.  
This is a massive advantage compared to protection principles like overcurrent, or directional protectiondirectional overcurrent protection.  
In this slide, zones and time characteristics for relays RAB and RBC are given.  
I'd like also to address the issue of selection of a time delay of zones two, and three.  
You can ask yourself, "Why 300 milliseconds?" Why not, for example, five milliseconds, or why not one minute?  
Which would be practical, we select those values which have practical nature.  
So, we must make sure that there is a difference between the speed of operation, for example of relay RBC.  
Which operates instantaneously, and relay RAB which operates in zone two.  
So, technologically it is not very complicated to ensure that time delay of 300 milliseconds would be sufficient to ensure secure and reliable operation of distance relay.  
Moving forward, let us make a summary about stepped distance relay through the given example.  
In this example, a transmission network fed by two active networks is given.  
Transmission lines are protected using distant relays.  
Let us discuss distance relay at position J.  
You can find it is somewhere in the middle of the slide.  
This relay is by the distance relay and it is controlling it's circuit breaker J.  
So, we see also time coordinate and you can identify as you can see these purple lines, zone one of distance relay J.  
Which is covering, for example, 80 or 90% of this transmission line which is protected by distance relay J.  
Then for zone two, which is going beyond transmission line, and which is traditionally set to, for example, 120%, or %130 or even %150 of the length of the originaloriginally protected line.  
And you can also see zone three, but interestingly you see zone three forward, what means this is one looking at a line in question, which has to be protected, but also zone three reverse.  
So, modern release can offer different types of characteristics and operation of distance relay.  
So, in this case, as you can see zone three has it's forward and backward options.  
Which can be also properly set.  
But thenow I would like to that the zone three protection, which is considered as a back up protection it is traditionally so set, that it is covering the...lines which are connected to the end of the main line I mean, which we are protecting.  
But it should cover the longest connected line, and go beyond it.  
Through this example, you can conclude how distant protection actually flexible is.  
We will now discuss an example how to set distance relay RAB located at busbar A in the shown network.  
So, as you can see in this network we have line AB and then on busbar B, we have two extra lines with different length.  
Line BC is obviously longer than line BD.  
And when it comes to distance relay RAB we assume that it has three zones.  
And considering that the impedance of the protected line is for plus j30 the zone one should be set to 85% of this entire line length, what means 85% of it's whole impedance.  
You might ask yourself, "Why 85?  
Why not 90, or why not 70?" So, this is, I would say something what is enhanced on the protection engineer, who will make sure that we will have a sufficient margin through the end of the line.  
In this case we have decided to have covered 85% percent of the transmission line.  
And it has to do with the quality of instrument transformers and the quality of relay in question it's accuracy, how precise it is.  
But in this case, we decided to cover 85% of the transmission line and to protect it by zone one.  
End operation is after zero seconds.  
Zone two, 120% of the line, which we are protecting of the line AB.  
End operation after 300 milliseconds, or 0.3 seconds.  
And how to set zone three.  
So, zone three should be so set that it goes beyond all transmission lines.  
What means, in this specific case it must cover transmission line AB plus BC and go a little bit beyond.  
So in this case, let me see how we have achieved that.  
So we said, 100% of transmission line AB plus 150% of transmission line BC.  
So this is one of options which we can accept.  
End operation time, one second.  
Another option, so it's now up to you could be line AB plus line BC and altogether times, for example, 1.2, what means 120% of the whole length AB plus BC.  
So, I think that you see how actually we flexible are, when it comes to the selection of settings of distance relay.  
So, after discussing the above settings, let me actually explain how distance relay actually works.  
So, looking at transmission line AB, and let us assume that we have thought at 1.  
at the transmission line.  
And we analyse the operation of relay distance relay located at busbar A.  
The first thing is that this relay will detect the fault this is the first step.  
Traditionally, detection of the fault is based on the monitoring of current.  
So, if current goes beyond a certain threshold the fault is detected.  
The next step is fault direction.  
So, we then include also information about voltage and by combining voltage and current, we detect if the fault is in my zone, or what means forward, or behind me.  
If it is in my zone, if it is in front of me I will move forward with other steps.  
Otherwise, if, for example, the fault is somewhere behind me I will not consider it as like, my fault.  
The next step is fault type detection.  
What means is it a three phase fault?  
Is it a single line to ground fault, is it A to ground, B to ground or C to ground?  
Is it phase to phase to ground fault, and so on.  
When we know the fault type, andWhen we know that the fault is in my direction, if you like, we move forward and calculate the impedance to the fault and based on the impedance measured, follows an operation.  
If we are in zone one, we operate instantaneously, zone two, after one time delay and zone three, after even larger time delay.  
Of course, when it comes to operational zone three, traditionally, other relays will operate in zone three will practically not operate.  
It is just a backup in the case that the other relays just not operate, and it happens in the network and that's why we must rely on backup solutions.  
As I have already introduced relays are connected over instrument transformers Voltage and current transformers.  
So, this fact can create confusion between so called primary and secondary quantities (INAUDIBLE) relay settings.  
Let us discuss the network presented in this slide.  
So, we see one transmission line AB with distance relay RAB which is connected over CT and VT and which is controlling a circuit-breaker.  
This transmission line AB is from left-side connected to an active network.  
So, we have secondary fault impedance which is calculated through the formula given in this slide, and as you can see, it is a function of turn ratios of both CT and VT.  
Considering that traditionally CT ratio is, for example, 500 to 5A or VT, 20,000 to 69.3V.  
As you can see that these two ratios are different.  
And consequently, the conclusion is that impedance of the line or fault impedance seen on the secondary side is not the same like the one on the primary side.  
So, it can be concluded that turn ratios for both CTs and VTs are different so that the secondary quantities are different from primary quantities.  
And in this context, a protection engineer, when it comes to setting of distance relays, must be very careful when it comes to the selection of variables...  
I mean of settings of distance relay.  
So, in the previous case in which we analyse transmission line with impedance four plus J30, we firstly,...  
if we want to firstly use secondary variables, we have to convert this primary impedance which is four plus J30 to the secondary one which is 1.386 plus J10.395, and based on this variable, we can move forward with setting of different zones.  
For example, zone one setting is this case would be 1.17 plus J8.84.  
Just to let you know that these were very serious blackouts worldwide as a result of wrong settings.  
I was involved in a project in which, unfortunately, wrong settings were put into the relay; Instead of secondary, primary settings were put and unfortunately, relay didn't operate properly.  
And this has caused, as I said, actually partial blackout.  
I would like to discuss now, how distance relay characteristics are presented and analysed.  
For this purpose, let us analyse this transmission line AB; This transmission line has its resistance and inductance, so R plus JX.  
So, this line impedance can be presented in the complex R-X diagram or R-X plane.  
So, by using this complex R-X diagram, we are presenting not only line impedance but also distance relay characteristics.  
So, I'll go to this topic further in my next slide.  
Before we move forward, let us note that the ratio E over I at the relay location is an impedance under all circumstances.  
When the fault occurs, this impedance assumes the value Zf.  
So, the ratio E over I is known as the apparent impedance seen by the relay.  
So, a relay always sees some impedance but the idea is that the impedance seen by the relay is also the impedance to the fault location.  
And it is ensured by the proper selection of input quantities, input variables to relay.  
So, for the previously given network in which we had transmission line AB, we could create a diagram R-X diagram presented in this slide.  
So, we decided to have busbar A exactly in the centre of this diagram, and you can identify A to B is impedance of the transmission line.  
Then you can also see where the point S is It is behind this point.  
And you can also identify that given a fault F, it is somewhere in this zone one of the relay.  
And so in this context, you can see how different impedances can be put together in a single diagram and how actually we can create our understanding where the fault is at least on our transmission line.  
I have already introduced the importance of different types of faults.  
Importance for the proper operational distance relays.  
Let us make a review of all possible fault types which might occur on a three phase transmission line.  
For example, we can have one three phase fault that means line one, line two, line three.  
We can have three types of line to line faults.  
For example, AB, AC, or BC.  
Then we can have three types of line to line to ground faults, or last but not least, three types of phase to ground faults A ground, B ground and C ground.  
In each case, we have different relationships between voltages and currents which must be used to calculate by distance relay exactly the fault distance and fault...  
impedance to the fault.  
So, one option could be to have ten types of different relays for all ten types of faults; But this is definitely something what wouldn't be practical enough.  
That's why relay is intelligent and clever to detect the fault type and to select an appropriate formula based on which exactly the distance to the fault...  
I mean the impedance to the fault will be calculated.  
To properly and systematically assess different fault types, we need to be confident with power system analysis module and in particular, short circuit studies.  
The methodology for short circuit studies is based on the use of transformation matrix given in this slide.  
And definitely to show that you are aware about this matrix, this is a transformation matrix for transforming variables from the original ABC to symmetrical components '012' space.  
And from the symmetrical component space back to the original ABC space.  
  
  
  
# 4.2 Input Variables Selection  
--LECTURER:  
To ensure a correct operation over distance really, its input variables must be properly selected.  
They must be so selected that the apparent impedance measured by the relay is equal to the fault impedance or impedance of the fault.  
We are now focussed on the problem, fault type selection.  
So for a given fault type an appropriate combination of input variables must be undertaken.  
So actually we are going to the following issue, understanding of faults, faults type and mathematical modelling of different types of faults.  
Through this mathematical modelling which is known as short circuit analysis, we will come to answers which input variables must be used for specific fault types.  
For example.  
which combination of voltages and currents measured by relay should be used for a single line to ground fault?  
For example line A to ground fault or B to C to ground fault.  
For every fourth type and we have learned that we have ten fault types.  
One specific combination should be used.  
So this is our focus of this lecture now.  
To simplify our study how to select distance relay input variables for different fault types, let us analyse the single line diagram of a transmission line connecting two active networks presented in this slide.  
We are focussed on input variables of distance relay RAB which is protecting a line AB.  
We will now show the methodology for input variable selection for all possible fault types.  
Let us start with the three phase fault.  
Three phase fault is traditionally the fault which doesn't happen so often.  
And traditionally it is related to mistake which for example, speed gear is earthed in an earthed position and from unknown reasons a circuit breaker is connected and then suddenly the entire line is exposed to three phase fault.  
Such faults are really very, very rare but they are very easy to be assessed that's good news.  
For this type of fault the signal diagram presented in this slide can be drawn.  
So no negative and no zero sequence components because it's symmetrical case.  
This is a simple case so that you can derive the final equation for impedance on your own.  
The formula obtained, the final formula in the in the lower right corner is indicating that for calculation of impedance to the fault it is z one f it is positive sequence impedance.  
We need different combinations of voltages and currents.  
For example Ea minus Eb divided by Ea minus Ia minus Ib and so on and so on.  
So in principle just by dividing voltage...  
phase voltage by phase current one obtains impedance of the fault.  
So this is a very simple example but very useful for understanding how input variables for a specific fault type are selected.  
So again we have the networking question, in this network we have a transmission line.  
So this is the transmission line which is presented in this slide alright.  
And we are analysing which input variables are used for relay RAB.  
So when it comes to three phase fault we move to modelling of the network.  
The model is expressed to the single...  
through line diagram which you'll see in this slide, And based on this model we derive appropriate equations which are such that we create an expression for impedance of the fault.  
So this expression is actually telling us what should be input variables used for distance relay in the case of this type of fault, in this case three phase fault.  
Let us now move forward to the most common fault type, the phase to ground fault or single line to ground fault.  
We have three types of this faults it can be phase A to ground, phase B to ground or phase C to ground.  
From power system we have in this case all symmetrical components, zero sequence, positive sequence and negative sequence components.  
And in this slide, the entire derivation of the final equation for calculation of impedance of the fault what it means is that one f, one reference to a positive sequence is given in this slide.  
For your exercise make sure to derive this equation.  
It is known to you from the module power system analysis.  
So input variables from equation one should be phase...  
so we are talking about phase A to ground fault, that should be phase A voltage, phase A current and zero sequence measured by relay for this type of fault and multiplied by compensation factor, The formula for a compensation factor is also given.  
So I would like to point the compensation factor calculated by this formula, this is in principle a complex number.  
And it is calculated based on line parameters.  
So for a given transmission line which we want to protect, we calculate K based on its zero sequence and positive sequence parameters.  
This is very important.  
Let us move to phase to phase faults, note that in this case zero sequence component does not exist because there is no connection to ground.  
And note that equation given in the right lower corner is indicating which input variables should be used in this case.  
So considering that the fault is from B to C.  
In this case we have to use for example Eb minus Ec divided by IB minus IC.  
So this combination of input variables must be used and used according to this formula so that the impedance of the fault would be obtained.  
Finally let us just conclude that for the phase to phase to ground fault for example BC to ground fault we use the same input variables like in the case of phase to phase fault, I mean B to C.  
I have prepared in this slide an example for you.  
So let me discuss this example, in this example we consider the system represented by the single line diagram.  
This is by the way of three phase system.  
The system nominal voltage is 13.8kV, and the positive and zero sequence impedances are as shown in this figure.  
And our task is to verify the distance calculation equations for three phase fault, phase to phase and phase to ground faults.  
I am encouraging you to do that for a homework and considering that one transmission parameters are given and so just note that four plus j 40 is the distance between busbar A and the fault so that we actually already know what's the answer in all cases.  
For all cases we should obtain the result four plus j 40.  
So these should be the correct results.  
I am encouraging you to do that as homework and if not you can find out more details about this example in our tutorial.  
So by now we have been assumed that all faults, where so called metallic or moulded faults.  
That means fault without any resistance.  
But in reality faults are not metallic faults but followed by different types of resistances.  
For example tower footing resistance, or resistance which has random nature for example connection of a conductor to ground and ground can be a different material.  
It can be food, it can be sand, it can be water and so on and so on.  
And one phenomenon is electrical arc which traditionally follows faults.  
So all these mentioned phenomena have a resistive nature.  
And in this context instead of analysing pure metallic or bolted faults we have to cope with a fault over resistance which we call fault resistance.  
This fault resistance has an impact on the fault impedance or impedance seen by the relay.  
Let us analyse these effects in this slide.  
So by analysing what is happening at the point where we have a fault over resistance.  
We can see that first the impedance is measured by a relay located at busbar A.  
So we have a voltage drop across this fault resistance.  
Without remote and in feet, we would just have a voltage drop caused by the current measured by relay at busbar A.  
And in this case the fault would be practically extended by this resistive component which is also seen on this Rx diagram.  
And this is also practically the...  
that what is shown also through equation given.  
However, we traditionally have another in feet actually fault current coming from another side of the transmission line assuming that the line is connecting two active networks.  
So these remote and in feet is creating an extra voltage drop across the fault resistance.  
If these two currents I and I remote Ir are in phase, we would have an effect in which you have just horizontal extension of the impedance seen by relay.  
But the...  
these two currents are traditionally not in phase, that' why we have to...  
we have different options and difference as it is seen in this Rx diagram.  
So you can see what is the impact of a fault resistance.  
The impact is that the impedance seen by a relay, the fault impedance is different.  
And this must be considered when creating a distance protection characteristics.  
And when designing how distance really will operate.  
  
  
# 4.3 Types of Distance Relays  
--LECTURER:  
Let us now move forward to the topic types of distance relays.  
This topic has to do with characteristics of distance relays.  
So historically, we have experienced different types of distance relays, and let me discuss which types of distance relays can be found today.  
In this slide, four types of distance relay are presented.  
Impedance distance relay, admittance, reactance and quadrilateral.  
So, each of them is presented in this slide as you see number one two and three and four, and the interesting one is admittance relay, as you know admittance is inverse from resistance.  
That's why this characteristic is also called MHO.  
What is actually as you see inverse from OHM.  
That's quiet interesting curiosity.  
So how a relay operates if impedance measured by relay, is inside the characteristic the relay will operate.  
Otherwise it will block.  
For any, for example for admittance type relay, if the impedance measured is inside the characteristic, the relay will operate.  
Now the question is, if it is one, two or three.  
If it is outside, it will block and it will not operate.  
I would now like to discuss in more details the admittance distance relay.  
This is a very often relay characteristic which is used and the MHO relay or admittance relay is determined by the angle phi and its impedance setting.  
So please see the graph on the left side, in this graph firstly, the red line is line impedance characteristic, so it has certain RNX and the transmission line is line AB, line A is the left end and then point B is the right end.  
So the characteristic is so selected that it considers also effects of arc resistance or tower fort resistance, this is that what we call fault resistance.  
So that by selecting phi and this point P, which is determined by zone, zone one for example, we will in this way obtain point Q and based on A and Q, we could create...and phi...we could create this circle.  
And this would be an admittance distance relay characteristic.  
On the right side you see also few zones, zones one two and three, so that as we can see zone one is set to for example 80 or 90% of the entire line length AB, then you can also see zone two, this zone two goes beyond line AB, and it is also covering certain part of the next line connected to the originally protected line AB.  
And you can also see very interestingly selected zone three, don't be surprised that it is so selected, but that is an interesting in which relay looks both and operates as backup protection it looks both forward and in reverse direction.  
Quite elegant solution.  
I would personally recommend you to look at all these characteristics in the reference given.  
This is network protection and automation guide by ALSTOM...ALSTOM GRID.  
Quite a good book, however in my opinion, quite appropriate for those who are not beginners in the field of power system protection.  
Last but not least, let us analyse the quadrilateral distance relay characteristic.  
This kind of characteristic is a result of application of modern technology and application of microprocessor based distance relays.  
It's quite flexible, and I think that these images given, they are telling how flexible this kind of protection is.  
So on the left side, RX diagram for...in which we see all zones, zones one two and three, you can see for a given transmission line AB, how zone one should look like, zone B and zone C.  
So in this case definitely resistive faults are properly assessed and taken into account and we get also very flexible backup protection zone three, and zone two is as you can see also going beyond transmission line AB, going into transmission line BC.  
On the right side, you see also quite if you like, exotic characteristic, and you see something called load encroachment.  
So for a given quadrilateral characteristic or any characteristic of distance relay, what can happen particularly in the case of short and very overloaded transmission lines.  
So very short and very overloaded means that the impedance seen under normal operating conditions is voltage divided by current.  
So I said very loaded, what it means is this current is very high.  
So consequently, this voltage divided by current is a small number.  
It's actually a small impedance, which could also practically encroach the zone one characteristic for example.  
That's why we have this kind of load encroachment part which considers the fact that under normal loading conditions we have to exclude these impedances from the operational region of this quadrilateral distance relay.  
Quite interesting and indeed practical.  
In this slide, you can see different brands of relays, so they are traditionally manufactured by major companies like ABB or Cell or Siemens or GE and you can also look how the usually look like.  
As a matter of fact, all of them presented in this slide are digital relays and they are based on multiprocessor systems.  
Is practically like modern industrial PC, which is if you like doing the business, what means having input variables, what means voltages and currents, processing them, calculating voltage in phases, voltage and current phases and then calculating the unknown impedance of the fault.  
Thank you very much for listening my lecture on distance protection, I will see you in the next video.  
  
  
# 4.4 Distance Protection Schemes  
--LECTURER:  
Hello, welcome to this video.  
I would like to talk about one specific aspect of distance protection, it is distance protection schemes.  
From the perspective of operation of these in three ways and the concept of zones which are time-graded, zone one, zone two and zone three, their operation can be further optimised.  
The optimisation can be achieved using novel technology, for example, fast communication channels.  
So, I have already introduced that for a given transmission line protected by distance relays, we have one distance relay located at one end another distance relay connected to the other end, by creating a communication channel between these two, distance relays, we could improve their operation.  
So, we will analyse how using concept of distance protection schemes we can achieve that.  
Let us first recapitulate how distance relays are set.  
In the left figure of this slide, the single line diagram of a network is presented and on the diagram, distance relay A can be identified and this relay is sitting next to busbar A, so, we see transmission line A, B and distance relay at the left line terminal are the terminal A.  
Note that distance relay B is also protecting the same line but looking in opposite direction.  
So, functionality of relays can be represented by using logical diagrams or logical components and or components or components indicating time delay.  
So, look at the trip circuit logic in which the trip signal is a result of operation of all three possible zones.  
So, zone one or zone three or zone two.  
Zone two is time delayed by time-delay allocated for this zone and the zone three is time delayed allocated for this zone.  
So, having any of these signals, high or logical one, we will have a trip signal.  
We have a number of issues with the standard distance protection application and the standard concept of time graded zones.  
One of issues is that the conventional time-stepped distance protection cannot be tolerated in some applications for two main reasons.  
For example, there is a need for faster operation of zone two, otherwise, we could have problems with stability of the electrical power system or we could have problems with high-speed autoreclosing.  
So, high-speed autoreclosing is indicating that we have need for high-speed, and high-speed, unfortunately, cannot achieved by slowed down zone two.  
For example, we have two networks and these two networks are connected to each other and operating properly, and if we have autoreclosing function which has to be slowed down, when it comes to operation of autoreclosing, we could have a problem of stable reconnection of these two networks which could, unfortunately, have voltages or voltage phasors which have different angles.  
So that, reconnection of these two networks wouldn't be appropriate and would be a problem.  
To cope with this kind of problems, you need schemes of protection that compare the conditions at the two ends of the feeder simultaneously, positively identify whether the fault is internal or external to the protected section and provide high-speed protection for the whole feeder length.  
So, I'd like to explore options.  
If we would, somehow, be able to accelerate the operation of zone two or if we could have better solution for a coordinated operation between these two relays, distance relays, located at two ends of transmission line.  
So, if we have a communication channel, we could achieve that.  
So, let me now move to the next slide.  
In this slide, the so-called 'direct under-reach transfer tripping scheme' is presented.  
So, let us assume that the fault is not in the middle of transmission line, so, given a fault in the middle of transmission line, both relays would operate in zone one, but what if the fault is very close to one of these transmission lines, so that, one relay will operate in zone one and the other in zone two, that means that the selective operation would require operation of zone one of one relay and zone two of the other relay.  
So that, finally, the fault would be eliminated after the operation of zone two.  
What means, not instantaneously after zero seconds, but after time delay which can be, for example, 300 milliseconds or even more, 500 milliseconds.  
This can, as I already introduced, cause issues with, for example, stability of two networks which are connected on this transmission line or problems with high-speed autoreclosing function.  
So, let us analyse how this direct under-reach transfer tripping scheme works.  
So, if the fault has been recognised as zone one fault from one relay, you can see the logical block diagram on the left side.  
This signal would be directly sent to the OR gate which is then determining the trip signal, as you can see on the right side of the slide and logical diagram.  
So that, by this, what is happening?  
So, on the left side, zone one initialised the tripping of a circuit breaker and this circuit breaker will be tripped instantaneously.  
On the other hand, using communication channel which, as a matter of fact, must be very fast, we transfer the signal to the OR gate of the trip of the other relay, so that, we only lose the time for the transfer of this information from one relay to another relay.  
So, this transfer can be done, for example, within 5 milliseconds, so that, practically, we have close to instantaneous operation of both relays and opening of both circuit breakers.  
However, in the reality, we have opening of one relay, or one circuit breaker and after that, the second one, but, definitely faster than, for example, the time defined by the time-delay of zone two.  
So, this is quite an elegant way how to solve the problem of the fact that zone two is slowed down compared to zone one.  
When it comes to security and the reliability of power system protection, these are different ways to improve both of them.  
So, we are very happy to transfer signal from one relay to another relay to encourage another relay to operate faster but we would really like to be really confident that this entire operation is secure and reliable, that's why the following 'permissive under-reach transfer tripping scheme' has been designed.  
So, from the left relay, you can see that the zone one signal is transferred directly to relay on the other side, but you will see that this signal is received but is time delayed for a given time-delay.  
So, we need this time-delay, I will explain why.  
At the same time, you see the final trip signal, I mean caused by the relay from coming from the left side, is obtained from one end-gate and this end-gate has two inputs, one is zone two and the other is the signal received and time delayed from the left relay.  
So, by combining these two, we make sure that relay on the right side will operate.  
So, what is that would be achieved by this?  
We make sure that, definitely, the right relay sees the fault in zone two and this is then something what is making this scheme more secure and more reliable.  
Thank you very much for watching this video about distance protection schemes and let us move to the next one.  
  
  
  

