import os
from building import *

objs = []
cwd  = GetCurrentDir()
# print('cwd:', cwd)

for item in os.listdir(cwd):
    sconsfile = os.path.join(cwd, item, 'SConscript')
    # print('item:', item, 'sconsfile:', sconsfile)
    if os.path.isfile(sconsfile):
        objs += SConscript(sconsfile)

Return('objs')
