Description

The production of a high brillance muon beam is one of the most important challenge for the future of Particle Physics. A particularly interesting idea consists of shooting high energy positrons on a target, aiming at the production of muons by means of the process . To mimize the divergence of the resulting "muon beam", the positrons energy is chosen so that the reaction occurs close to threshold (assuming the electrons in the target to be at rest). The main goal of this project is to produce a Monte Carlo simulation of such a process.

Details

Assume a  meter long,  Tesla dipole magnet is placed after the target. Assume a number of tracking detectors can be placed before the target, after the target before the magnet (one line) and after the magnet (two lines, one for positive the other for negative muons); those could be made of silicon pixels, with a single-hit resolution varying from 50 to 200 .
Try to address the following items keeping in mind that money matters (i.e. you cannot buy an infinite number of detectors and the smaller the single-hit resolution the higher the cost) and that the layout of the experiment has to be as compact as possible (say whithin 20 m).

Define the sizes of the various detectors, such that all the particles traverse them (i.e.  detector acceptance);
have each event of the synthetich dataset "interacting" with the detectors, i.e. generate a dataset with the hits (properly smeared due to detector resolutions) left by particles crosssing each detector. That should correspond to the actual measurments gathered by the experiment;
add some random noise to such measurements (e.g. for each detector accordingly to poisson statistic of mean about 1);
develop an algorithm to track the particles, both the incoming positrons and the outgoing muons.
keep in consideration the fact that the two muons emerge synchronously from the target: how small the pitch (the distance between individual pixels) have to be of the detectors prior to the magnet? If that is too small, adjust the tracking algorithm accordingly (i.e. the reconstruct muon tracks could share hits in those detectors)
compute the resolution of the muon momenta and of the ;
