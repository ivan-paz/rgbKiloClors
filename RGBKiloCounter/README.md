# kiloCounter 

## Quick start
1. install scikit-image library (this depends on your operation system).

1.1 You might also need to install pandas library.

The main script to be executed in a terminal is:

python kiloColorCounter.py <args> 

description='Kilocounter tracks R, G, B colors from kilobots video frames'

the expected arguments are:


'kilobots', type=int, metavar='n_kilobots', help='the number of kilobots to expect in the images'

'-i', '--input', type=str, metavar='',
                    help='folder containing the images to process, default is Images', default='Images'
                    
'-o', '--output', type=str, metavar='',
                    help='name of the output file, default is results.csv', default='results.csv'
                    
'-e', '--evil_dir', type=str, metavar='',
                    help='folder to copy the evil images, default is Evil', default='Evil'

Evil images are those where the number of kilobots does not match the expected number.
                    
'-n', '--n_processors', type=int, metavar='',
                    help='the number of threads to parallelize the computation, default is os.cpu_count()', default=os.cpu_count()
                    
'-r', '--results_dir', type=str, metavar='',
                    help='folder to copy all the images, default is None', default=None
                    
You might to create the default folders in your working directory.
