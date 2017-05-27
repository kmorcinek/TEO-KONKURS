``` ini

BenchmarkDotNet=v0.10.5, OS=Windows 10.0.15063
Processor=Intel Core i7-4710MQ CPU 2.50GHz (Haswell), ProcessorCount=8
Frequency=2435773 Hz, Resolution=410.5473 ns, Timer=TSC
  [Host]            : Clr 4.0.30319.42000, 32bit LegacyJIT-v4.7.2046.0
  LegacyJit-Clr-X86 : Clr 4.0.30319.42000, 32bit LegacyJIT-v4.7.2046.0

Job=LegacyJit-Clr-X86  Jit=LegacyJit  Platform=X86  
Runtime=Clr  

```
 |                    Method |     Mean |     Error |    StdDev | Scaled | ScaledSD |     Gen 0 | Allocated |
 |-------------------------- |---------:|----------:|----------:|-------:|---------:|----------:|----------:|
 |  Test_v_0_9_transformator | 2.469 ms | 0.0039 ms | 0.0035 ms |   1.00 |     0.00 | 1408.0729 |   4.33 MB |
 | Test_v_0_10_transformator | 2.436 ms | 0.0122 ms | 0.0114 ms |   0.99 |     0.01 | 1405.9896 |   4.33 MB |
 | Test_v_0_11_transformator | 2.467 ms | 0.0085 ms | 0.0079 ms |   1.00 |     0.00 | 1407.0313 |   4.33 MB |
 | Test_v_0_12_transformator | 2.571 ms | 0.0088 ms | 0.0083 ms |   1.04 |     0.00 | 1521.8750 |   4.69 MB |
 |  Test_v_1_1_transformator | 2.422 ms | 0.0492 ms | 0.0460 ms |   0.98 |     0.02 | 1398.6979 |   4.33 MB |
 |  Test_v_1_2_transformator | 2.431 ms | 0.0208 ms | 0.0195 ms |   0.99 |     0.01 | 1399.7396 |   4.33 MB |
 |  Test_v_2_0_transformator | 2.970 ms | 0.0073 ms | 0.0061 ms |   1.20 |     0.00 | 1398.6979 |   4.33 MB |