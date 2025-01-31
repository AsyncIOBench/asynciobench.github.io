# High-Performance I/O Benchmark

This project provides a benchmark tool to compare the performance of different I/O engines for storage systems. The main goal is to evaluate how well each engine handles tasks like random read, random write, and mixed read-write operations in terms of IOPS, latency, and throughput.

### Supported I/O Engines
- **libaio**: A traditional Linux asynchronous I/O library.
- **io_uring**: A newer, more efficient asynchronous I/O interface in Linux.
- **SPDK (Storage Performance Development Kit)**: A user-space framework for high-performance I/O, designed especially for NVMe drives.

### Features
- Compares I/O performance metrics: **IOPS**, **Latency**, and **Bandwidth**.
- Results are displayed in tables and charts for easy comparison.
- Allows testing with different thread configurations (1 thread and 4 threads).

### How the Benchmarking Was Done
The tests were conducted using the following hardware configuration:
- **CPU**: 8-core Intel Xeon processor
- **RAM**: 32 GB
- **Storage**: NVMe SSD (Samsung 970 Pro)
- **Test Duration**: Each test lasted for 10 seconds
- **Tool Used**: fio (Flexible I/O Tester)

### Key Performance Metrics
- **IOPS** (Input/Output Operations Per Second): Indicates the speed of I/O operations.
- **Latency (µs)**: Measures the time taken to complete an I/O request.
- **Bandwidth (MiB/s)**: Represents the data throughput during read/write operations.

## Team
- [Iman Mohammadi](https://github.com/Imanm02)
- [Kiarash Joolaei](https://github.com/KiaJJ)
- [Sobhan Asadi](https://github.com/SobhanAsadi)