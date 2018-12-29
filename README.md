Unnecessarily elaborate because based on a real-life puzzle: why does UserDefaults seem to fall behind?

The answer, however, probably has nothing to do with the details of the code, but rather with my testing procedure. If you run this example repeatedly on simulator from Xcode (i.e. run, hit button repeatedly, stop, run again immediately, hit button repeatedly, etc.), you'll see that UserDefaults does indeed fall behind, but this seems to be because _UserDefaults saving takes time_. The solution is to count to 10 slowly before stopping and running again.
