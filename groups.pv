import subprocess
gam = "C:\\users\\backend\\desktop\\gam-64\\gam.exe"
output = 'output.txt'

with open('groups.txt', 'r') as f:
    for line in f:
        n = line.rstrip() #delete \n which will screw gam up
        switch = ' print group-members group {0} membernames'.format(n)
        p = subprocess.check_output(gam + switch)
        with open(output, 'a') as g:
            g.write(p)

