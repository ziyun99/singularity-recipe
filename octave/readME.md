# Singularity recipe for Octave-6.2.0

### References (for Octave dependencies): 
- Ubuntu: http://wiki.octave.org/Octave_for_Debian_systems
- CentOS: http://wiki.octave.org/Octave_for_Red_Hat_Linux_systems
- Build from source: http://wiki.octave.org/Building


### To pull images we built (from Cloud Library):
- Ubuntu 18.04: `singularity pull library://ziyun99/octave/ubuntu18.04-octave:6.2.0`
- CentOS 7: `singularity library://ziyun99/octave/centos7-octave:6.2.0`


### Other references:
- Official GNU-Octave docker/singularity image:
    - Source: https://github.com/gnu-octave/docker
    - Command: `singularity pull docker://gnuoctave/octave:6.2.0`
    
    - Source: https://github.com/gnu-octave/GNU-Octave-ILP64-Singularity
    - Command: `singularity pull library://siko1056/default/gnu_octave:5.2.0`
    
- Official Sylabs Octave singularity image: 
    - Source: https://github.com/sylabs/examples/tree/master/lang/octave
