# CNCFuzzer-datasets

好的 👍 下面给您一个适合 **研究数据集发布** 的 README 模板，结构清晰，便于其他研究者快速理解和使用 CNCFuzzer 数据集。您可以根据实际情况填充内容：

------

# CNCFuzzer Dataset

## Overview

This repository provides the dataset used in the paper:
 **“CNCFuzzer: Directed Black-box Fuzzing of Computer Numerical Control Systems Based on Message Behaviour Guidance” (TOSEM)**.

------

## Contents

- **`/CPM-dataset/`**: Current (electrical) data collected from CNC devices, used to train models for device state recognition.
- **`/MMG-dataset/`**: Proprietary protocol traffic dataset, used for message generation and fuzzing test case construction.

------

## Dataset Statistics

- Total records: **705,361**
- Protocol: **EzSocket (TCP-based application layer protocol)**
- Functional categories: **19** (e.g., library handle, axis/spindle data management, program management, tool data management, waveform diagnosis, PMC management, etc.)
- Payload sizes: **40 bytes, 46 bytes, 68 bytes, 216 bytes, ...**

------

## Coverage

The dataset includes the majority of **high-risk operation APIs** (e.g., axis/spindle data management, program management), which are most relevant for vulnerability discovery.
 Some APIs are not included, such as:

- Deprecated APIs,
- APIs with complex state machines (e.g., CNC file data),
- APIs for special devices (e.g., punch press, laser, wire cut) not available in our lab.

------

## Citation

If you use this dataset in your research, please cite:

```
@article{TBD

}
```

------

## Contact

For questions or requests regarding this dataset, please contact:
Zedong Li – lizedong@iie.ac.cn