# Rubik's Cube Project

A C++ Rubik's Cube simulator and solver playground focused on cube representation, move execution, and search-based solving strategies.

## ✨ Highlights

- Multiple cube state representations:
	- 1D array
	- 3D array
	- Bitboard
- Standard cube moves and face rotations (`R`, `L`, `U`, `D`, `F`, `B` and variants)
- Solver implementations (BFS, DFS, IDDFS, IDA*)
- Pattern database components for faster heuristic solving
- Scanner module scaffold for future OpenCV-based cube input

## 🧠 Why This Project

This project is a practical way to learn:

- Rubik's Cube notation and transformations
- State modeling trade-offs
- Search algorithms and heuristic optimization
- C++ project structure for algorithm-heavy systems

## 📁 Project Structure

```text
RubiksCubeProject/
├── CMakeLists.txt
├── main.cpp
├── Model/
│   ├── RubiksCube.cpp
│   ├── RubiksCube.h
│   ├── RubiksCube1dArray.cpp
│   ├── RubiksCube3dArray.cpp
│   └── RubiksCubeBitboard.cpp
├── Solver/
│   ├── BFSSolver.h
│   ├── DFSSolver.h
│   ├── IDDFSSolver.h
│   └── IDAstarSolver.h
├── PatternDatabases/
│   ├── CornerDBMaker.cpp
│   ├── CornerDBMaker.h
│   ├── CornerPatternDatabase.cpp
│   ├── CornerPatternDatabase.h
│   ├── PatternDatabase.cpp
│   ├── PatternDatabase.h
│   ├── NibbleArray.cpp
│   ├── NibbleArray.h
│   ├── PermutationIndexer.h
│   ├── math.cpp
│   └── math.h
├── Scanner/
│   ├── CubeScanner.cpp
│   └── CubeScanner.h
└── bits/
    └── stdc++.h
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/RATAN1369/RubiksCubeProject.git
cd RubiksCubeProject
```

### 2. Configure and build (CMake)

```bash
cmake -S . -B build
cmake --build build --config Release
```

### 3. Run

Run the executable produced in the `build` directory.

On single-config generators (Make/Ninja), it is usually:

```bash
./build/RubiksCubeProject
```

On multi-config generators (Visual Studio), it is usually:

```powershell
.\build\Release\RubiksCubeProject.exe
```

## 🔧 Current Status

- Core cube modeling is in place
- Solvers are being expanded and tuned
- Pattern database support is present and evolving
- Camera-based scanning integration is planned

## 🗺 Roadmap

- Improve solver performance and benchmarks
- Add richer command-line interaction
- Integrate OpenCV scanning pipeline
- Add tests for move correctness and solver validity

## 🤝 Contributing

Contributions are welcome. If you'd like to improve algorithms, add tests, or help with scanner integration, open an issue or submit a pull request.

## 📜 License

Add your preferred license file (for example, MIT) to clarify usage and distribution terms.
