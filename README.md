1. Creating a worker pool which will listen on an input buffered channel waiting for jobs to be assigned.

2. The jobs are added to the input buffered channel.

3. After complition of the job the results are written up to an output buffered channel.

4. Finally result is readed and printed from the output buffered channel.

5. There are two go routines go allocate() and go results() where jobs are send to the input bufferd channel jobs and after calculation the result is recieved into the output buffered channel respectively.