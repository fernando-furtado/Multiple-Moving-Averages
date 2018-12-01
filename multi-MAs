//@version=3
study(title="Multiple Moving Averages", shorttitle="Mult. MAs", overlay=true)

// Super simple script integrating three moving averages within only one script. It's gonna help you to keep your chart cleaner while saving two spots for other indicators you may​ like. Try it out and let me know what you think.
// The script also allows you to switch between Simple Moving Averages and Exponential Moving Averages for each line you want to plot.


// Simple trading strategy:
// Buy/Sell crossover of the MAs. Buy/Sell when fast MA crosses medium MA, double down when medium MA crosses slow MA.

// Combinations of trading strategies are usually a good idea.

// Tips
// BTC: 33RUY4AXBEL89gEsoqDpXRgvdZWePhLrqc
// LTC: M9mBqVhxWNuZuCPEsrRtH3ygxNYnCdMEki
// ETH: 0x1D3E1701F1A0C379e7Fcb60BADBcd14AcE8160c4
// DASH: XnKHHcmhZmR2SAqavP1x6FbEBrqTYa4kTk

// Trade wise and be careful.

SMA_EMA = input(true, "sma/ema")
len = input(50, minval=1, title="Length")
src = input(close, title="Source")
out = sma(src, len)
outE= ema(src, len)
plot((SMA_EMA ? out: outE), color=red, title="MA Fast", linewidth=1)

SMA_EMA1 = input(true, "sma/ema")
len1 = input(100, minval=1, title="Length")
src1 = input(close, title="Source")
out1 = sma(src1, len1)
outE1= ema(src1, len1)
plot((SMA_EMA1 ? out1: outE1), color=blue, title="MA Medium", linewidth=2)

SMA_EMA2 = input(true, "sma/ema")
len2 = input(200, minval=1, title="Length")
src2 = input(close, title="Source")
out2 = sma(src2, len2)
outE2= ema(src2, len2)
plot((SMA_EMA2 ? out2: outE2), color=green, title="MA Slow", linewidth=3)
