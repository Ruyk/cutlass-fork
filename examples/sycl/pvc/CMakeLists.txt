# Copyright (c) 2024 - 2025 Codeplay Software Ltd. All rights reserved.
# SPDX-License-Identifier: BSD-3-Clause
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions are met:
#
# 1. Redistributions of source code must retain the above copyright notice, this
# list of conditions and the following disclaimer.
#
# 2. Redistributions in binary form must reproduce the above copyright notice,
# this list of conditions and the following disclaimer in the documentation
# and/or other materials provided with the distribution.
#
# 3. Neither the name of the copyright holder nor the names of its
# contributors may be used to endorse or promote products derived from
# this software without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.


cutlass_example_add_executable(
  pvc_gemm
  pvc_gemm.cpp
)

cutlass_example_add_executable(
  pvc_gemm_with_epilogue_relu
  pvc_gemm_with_epilogue_relu.cpp
)

cutlass_example_add_executable(
  pvc_gemm_with_epilogue_gelu
  pvc_gemm_with_epilogue_gelu.cpp
)

cutlass_example_add_executable(
  pvc_gemm_with_epilogue_lincombdeeltact
  pvc_gemm_with_epilogue_lincombdeeltact.cpp
)

cutlass_example_add_executable(
  pvc_gemm_with_per_row_bias
  pvc_gemm_with_per_row_bias.cpp
)

cutlass_example_add_executable(
  pvc_collective_builder
  pvc_collective_builder.cpp
)

cutlass_example_add_executable(
  pvc_gemm_streamk
  pvc_gemm_streamk.cpp
)

add_subdirectory(flash_attention_v2)

cutlass_example_add_executable(
  pvc_gemm_mixed_dtype
  pvc_gemm_mixed_dtype.cpp
)
