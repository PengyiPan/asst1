1.
2.
    | Threads        | Time           | Speedup  |
    | ------------- |:-------------:| -----:|
    | 1     | 380.777 ms | 1.00x |
    | 2     | 193.828 ms | 1.96x |
    | 3     | 233.276 ms | 1.63x |
    | 4     | 158.164 ms | 2.41x |
    | 5     | 155.980 ms | 2.44x |
    | 6     | 120.083 ms | 3.26x |
    | 7     | 114.639 ms | 3.42x |
    | 8     | 98.164 ms | 3.91x |

3.
    ```
    ❯ for i in {2..8}
    do
    ./mandelbrot -v 1 -t $i
    done
    [mandelbrot serial]:            [386.646] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=196 ms
    thread1 time used=197 ms
    thread0 time used=195 ms
    thread1 time used=196 ms
    thread0 time used=195 ms
    thread1 time used=196 ms
    thread0 time used=195 ms
    thread1 time used=196 ms
    thread0 time used=195 ms
    thread1 time used=196 ms
    [mandelbrot thread]:            [195.975] ms
    Wrote image file mandelbrot-thread.ppm
                                    (1.97x speedup from 2 threads)
    [mandelbrot serial]:            [385.677] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=77 ms
    thread2 time used=78 ms
    thread1 time used=238 ms
    thread0 time used=76 ms
    thread2 time used=77 ms
    thread1 time used=237 ms
    thread0 time used=76 ms
    thread2 time used=77 ms
    thread1 time used=237 ms
    thread0 time used=77 ms
    thread2 time used=77 ms
    thread1 time used=238 ms
    thread0 time used=76 ms
    thread2 time used=77 ms
    thread1 time used=237 ms
    [mandelbrot thread]:            [237.133] ms
    Wrote image file mandelbrot-thread.ppm
                                    (1.63x speedup from 3 threads)
    [mandelbrot serial]:            [383.625] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=36 ms
    thread3 time used=37 ms
    thread1 time used=160 ms
    thread2 time used=161 ms
    thread0 time used=37 ms
    thread3 time used=37 ms
    thread1 time used=159 ms
    thread2 time used=159 ms
    thread0 time used=38 ms
    thread3 time used=38 ms
    thread1 time used=160 ms
    thread2 time used=160 ms
    thread0 time used=38 ms
    thread3 time used=38 ms
    thread1 time used=160 ms
    thread2 time used=160 ms
    thread0 time used=37 ms
    thread3 time used=37 ms
    thread1 time used=159 ms
    thread2 time used=159 ms
    [mandelbrot thread]:            [159.871] ms
    Wrote image file mandelbrot-thread.ppm
                                    (2.40x speedup from 4 threads)
    [mandelbrot serial]:            [384.996] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=17 ms
    thread4 time used=17 ms
    thread1 time used=101 ms
    thread3 time used=101 ms
    thread2 time used=157 ms
    thread0 time used=17 ms
    thread4 time used=17 ms
    thread1 time used=100 ms
    thread3 time used=101 ms
    thread2 time used=157 ms
    thread0 time used=29 ms
    thread4 time used=17 ms
    thread1 time used=102 ms
    thread3 time used=102 ms
    thread2 time used=157 ms
    thread0 time used=17 ms
    thread4 time used=17 ms
    thread1 time used=101 ms
    thread3 time used=102 ms
    thread2 time used=157 ms
    thread0 time used=17 ms
    thread4 time used=17 ms
    thread1 time used=101 ms
    thread3 time used=102 ms
    thread2 time used=157 ms
    [mandelbrot thread]:            [157.005] ms
    Wrote image file mandelbrot-thread.ppm
                                    (2.45x speedup from 5 threads)
    [mandelbrot serial]:            [385.962] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=10 ms
    thread5 time used=12 ms
    thread1 time used=67 ms
    thread4 time used=67 ms
    thread2 time used=120 ms
    thread3 time used=122 ms
    thread0 time used=12 ms
    thread5 time used=12 ms
    thread1 time used=69 ms
    thread4 time used=70 ms
    thread3 time used=122 ms
    thread2 time used=122 ms
    thread0 time used=12 ms
    thread5 time used=12 ms
    thread1 time used=67 ms
    thread4 time used=67 ms
    thread2 time used=119 ms
    thread3 time used=120 ms
    thread0 time used=12 ms
    thread5 time used=12 ms
    thread1 time used=67 ms
    thread4 time used=67 ms
    thread2 time used=119 ms
    thread3 time used=120 ms
    thread0 time used=10 ms
    thread5 time used=10 ms
    thread1 time used=67 ms
    thread4 time used=67 ms
    thread2 time used=119 ms
    thread3 time used=120 ms
    [mandelbrot thread]:            [120.314] ms
    Wrote image file mandelbrot-thread.ppm
                                    (3.21x speedup from 6 threads)
    [mandelbrot serial]:            [385.325] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=8 ms
    thread6 time used=10 ms
    thread1 time used=45 ms
    thread5 time used=50 ms
    thread2 time used=86 ms
    thread4 time used=90 ms
    thread3 time used=114 ms
    threadthread06 time used= time used=9 ms9 ms
    
    thread1 time used=45 ms
    thread5 time used=47 ms
    thread2 time used=86 ms
    thread4 time used=87 ms
    thread3 time used=114 ms
    thread0 time used=9 ms
    thread6 time used=10 ms
    thread1 time used=45 ms
    thread5 time used=47 ms
    thread2 time used=87 ms
    thread4 time used=88 ms
    thread3 time used=115 ms
    thread0 time used=9 ms
    thread6 time used=10 ms
    thread1 time used=45 ms
    thread5 time used=47 ms
    thread2 time used=86 ms
    thread4 time used=88 ms
    thread3 time used=115 ms
    thread0 time used=9 ms
    thread6 time used=10 ms
    thread1 time used=45 ms
    thread5 time used=47 ms
    thread2 time used=86 ms
    thread4 time used=88 ms
    thread3 time used=114 ms
    [mandelbrot thread]:            [114.646] ms
    Wrote image file mandelbrot-thread.ppm
                                    (3.36x speedup from 7 threads)
    [mandelbrot serial]:            [376.203] ms
    Wrote image file mandelbrot-serial.ppm
    thread0 time used=7 ms
    thread7 time used=7 ms
    thread1 time used=31 ms
    thread6 time used=34 ms
    thread2 time used=66 ms
    thread5 time used=67 ms
    thread3 time used=98 ms
    thread4 time used=98 ms
    thread0 time used=7 ms
    thread7 time used=7 ms
    thread1 time used=31 ms
    thread6 time used=34 ms
    thread2 time used=65 ms
    thread5 time used=66 ms
    thread4 time used=98 ms
    thread3 time used=99 ms
    thread0 time used=7 ms
    thread7 time used=7 ms
    thread1 time used=31 ms
    thread6 time used=34 ms
    thread2 time used=65 ms
    thread5 time used=67 ms
    thread3 time used=98 ms
    thread4 time used=98 ms
    thread0 time used=7 ms
    thread7 time used=7 ms
    thread1 time used=31 ms
    thread6 time used=31 ms
    thread2 time used=69 ms
    thread5 time used=69 ms
    thread3 time used=97 ms
    thread4 time used=97 ms
    thread0 time used=7 ms
    thread7 time used=7 ms
    thread1 time used=31 ms
    thread6 time used=34 ms
    thread2 time used=65 ms
    thread5 time used=67 ms
    thread3 time used=97 ms
    thread4 time used=98 ms
    [mandelbrot thread]:            [97.562] ms
    Wrote image file mandelbrot-thread.ppm
                                    (3.86x speedup from 8 threads)
    ```
    
    it looks like the work is not evenly distributed among threads?

4. The modified version achieved 7.09x speedup on view 1 and 6.96x speedup on view 2.

5. Comparing to 8 threads, 16 threads has around 2x more speed up, not significant tho.