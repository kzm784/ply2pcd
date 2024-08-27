
# ply2pcd ( PLY to PCD Converter )

This project provides a C++ program that converts PLY files to PCD files using the Point Cloud Library (PCL).

## Prerequisites

Before building the project, make sure you have the following dependencies installed:

- GCC (version 7 or later)
- CMake (version 3.0.2 or later)
- Point Cloud Library (PCL) (version 1.7 or later)

### Installing PCL on Ubuntu

You can install PCL using the following commands:

\`\`\`bash
sudo apt-get update
sudo apt-get install libpcl-dev
\`\`\`

### Building the Project

1. **Clone the repository:**

   \`\`\`bash
   git clone https://github.com/yourusername/ply2pcd.git
   cd ply2pcd
   \`\`\`

2. **Create a build directory and navigate to it:**

   \`\`\`bash
   mkdir build
   cd build
   \`\`\`

3. **Run CMake to configure the project:**

   \`\`\`bash
   cmake ..
   \`\`\`

4. **Build the project:**

   \`\`\`bash
   make
   \`\`\`

### Running the Program

After successfully building the project, you can run the program using the following command:

\`\`\`bash
./ply2pcd -format [0|1] /path/to/input.ply /path/to/output.pcd
\`\`\`

- \`-format [0|1]\`: Specifies the output format. Use \`0\` for ASCII and \`1\` for binary (default is binary).
- \`/path/to/input.ply\`: Replace with the path to your input PLY file.
- \`/path/to/output.pcd\`: Replace with the desired output path for the PCD file.

### Example

Here is an example command to convert a PLY file to a PCD file in binary format:

\`\`\`bash
./ply2pcd -format 1 example.ply example.pcd
\`\`\`
