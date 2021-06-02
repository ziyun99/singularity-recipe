# Singularity recipe for Octave-6.2.0

Singularity image of [GNU Octave](https://www.gnu.org/software/octave/) for high-performance computing (HPC).

### To build from definition files:
- Requirements: [Singularity](https://sylabs.io/) installed, root privileges, good internet connection, about 10 GB of free hard disk space, about 2 hours of time (system dependent)
- Ubuntu 18.04: `singularity build ubuntu18.04_octave-6.2.0.sif ubuntu18.04_octave-6.2.0.def`
- CentOS 7: `singularity build centos7_octave-6.2.0.sif centos7_octave-6.2.0.def`

### To pull the images we built (from Cloud Library):
- Ubuntu 18.04 (2.1GB): `singularity pull library://ziyun99/gnu-octave/ubuntu18.04_octave-6.2.0:v0` 
- CentOS 7 (1.7GB): `singularity pull library://ziyun99/gnu-octave/centos7_octave-6.2.0.def:v0`

### To run the images:
- `singularity run octave_image.sif` starts a CLI session.
- `singularity run octave_image.sif --gui` starts a GUI session.
- `singularity shell octave_image.sif` starts an interactive terminal.
- `singularity exec octave_image.sif octave my_file.m` runs the container with the script as input.

### References (for Octave dependencies): 
- Ubuntu: http://wiki.octave.org/Octave_for_Debian_systems
- CentOS: http://wiki.octave.org/Octave_for_Red_Hat_Linux_systems
- Build from source: http://wiki.octave.org/Building


### Other references:
- Official GNU-Octave docker/singularity image:
    - Source: https://github.com/gnu-octave/docker
    - Command: `singularity pull docker://gnuoctave/octave:6.2.0`
    
    - Source: https://github.com/gnu-octave/GNU-Octave-ILP64-Singularity
    - Command: `singularity pull library://siko1056/default/gnu_octave:5.2.0`
    
- Official Sylabs Octave singularity image: 
    - Source: https://github.com/sylabs/examples/tree/master/lang/octave
