# Seismic Labratory for Imaging and Modeling ![SLIM logo](images/slim.gif) 

## SLIM-tutorials - ML4Seismic 2024

Partners of ML4Seismic, please follow the below instructions to access the SLIM Lab tutorials. 

The tutorial sessions are scheduled to be held on Friday Nov 15. The entire meeting schedule can be found [here](https://slim.gatech.edu/content/ml4seismic-partners-meeting-2024)

1. Navigate to our server at [`https://slim-tutorials.org/`](https://slim-tutorials.org/)
2. Log in with your provided username. Please create a NEW password on your first login

![Login Preview](images/login.png)

3. Open a terminal 

![Terminal Location Preview](images/terminal.png)

4. Copy and paste the below commands into the terminal:

```
git clone https://github.com/turquoisedragon2926/SLIM-tutorials.git
julia -e 'using Pkg; Pkg.add("IJulia");'
/opt/julia-1.8.5/bin/julia -e 'using Pkg; Pkg.add("IJulia");'
cp -r ~/.local/share/jupyter/kernels/julia-1.10/ ~/.local/share/jupyter/kernels/julia-1.8
sed -i 's|1.10.4|1.8.5|; s|/opt/julia-1.10.4/bin/julia|/opt/julia-1.8.5/bin/julia|' ~/.local/share/jupyter/kernels/julia-1.8/kernel.json

export OMP_NUM_TREADS=1
export JULIA_NUM_THREADS=1
```

4. Access the required notebook using the directory navigator on the left panel

![Directory Location Preview](images/directory.png)

5. Select the current kernel on the top right

![Kernel Location Preview](images/kernel.png)

5. Select julia to be your active kernel from the list

![Julia Kernel Preview](images/julia.png)

6. Follow along with the speaker and enjoy!

If you do not have access to a username or have any trouble following the instructions, please talk to a SLIM lab associate.
