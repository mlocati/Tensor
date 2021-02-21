# FAQ
Here you will find answers to the most frequently asked questions.

## Is the Tensor extension multithreaded?
Yes, certain operations can be decomposed into sub routines and executed in parallel using multithreading. With that said, the Tensor extension makes use of many optimizations in addition to multithreading which tends to keep the main thread well saturated already. Thus, increasing the number of threads may not give you better performance.

To set the number of threads available to the extension:

```php
use Tensor\Settings;

Settings::setNumThreads(4);
```

## Is the Tensor extension vectorized?
Yes, the extension will use vectorized or SIMD instructions whenever possible. The type of registers used by your CPU under the hood will depend on your computer's architecture.

## Does Tensor support n-d array operations?
Not yet, however we plan to add a strided n-d array implementation in a future release.

## How can I contribute to the project?
Anyone is welcome to contribute to Rubix ML. See the [CONTRIBUTING](https://github.com/RubixML/ML/blob/master/CONTRIBUTING.md) guide in the project root for more info.

## How can I become a sponsor?
Check out our funding sources [here](index.md#funding) and consider donating to the cause.
