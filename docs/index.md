In the context of source separation solutions for virtual reality (VR) applications, several techniques in the spherical harmonic domain (SH) have been proposed in the literature. The performance of such methods is limited under high reverberation conditions and the rendering of the obtained spatial sound is fixed to the recording location only. Recently, novel sound field works in the literature proposed a global representation that enables both the estimation of the direct sound (exterior field) and the reconstruction in locations different from the acquisition ones. In this paper, we propose a signal processing framework based on Multichannel Non-Negative Matrix Factorization (MNMF) in the SH domain that operates directly over the exterior field coefficients enabling the reconstruction of the direct sound field of the separated sources. To evaluate our proposal, we compared with other state-of-the-art source separation approaches using several setups and including different reverberation conditions, showing promising results in terms of SDR metrics.

### Method
<!--  ![Image](figures/pipeline.png) -->

# Listening tests
Audio examples will be available soon.
<!--- Here below we report some audio examples along with the spectrogram of the signals. <br>
For each example [...]. <br>
We compare the results of the proposed method with the FastMNMF and ILRMA.
--->

<!-- FIRST EXAMPLE -->
<table style="width: 100%; table-layout: fixed; word-wrap: normal;">
  <!-- SETUP -->
  <tr> 
    <th colspan="8" style="text-align:center;">EXAMPLE 1: 4 HOMs, 2 Female sources Mixture <audio controls><source src="examples/exs1/2source/1position/4array/30/mix_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio></th>
  </tr>
  <tr>
    <td>
      Source position: 1 <br>
      T60: 0.3[s]<br>
    </td>
    <td>
      Estimated Exterior field (input of MNMF algorithms)
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/input_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 1 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/1order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/1order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 2 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/2order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/2order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 3 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/3order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/3order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      ILRMA <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/ilrma_est_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/ilrma_est_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      FastMNMF <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/fast_source_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/fast_source_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      Exterior Field Reference <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/1order/estFede1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/1position/4array/30/1order/estFede2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
  </tr> 
</table>

<!-- SECOND EXAMPLE -->
<table style="width: 100%; table-layout: fixed; word-wrap: normal;">
  <!-- SETUP -->
  <tr> 
    <th colspan="8" style="text-align:center;">EXAMPLE 2: 8 HOMs, 2 Female sources Mixture <audio controls><source src="examples/exs1/2source/2_position/8_array/120/mix_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio></th>
  </tr>
  <tr>
    <td>
      Source position: 2 <br>
      T60: 1.2[s]<br>
    </td>
    <td>
      Estimated Exterior field (input of MNMF algorithms)
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/input_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 1 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/1_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/1_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 2 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/2_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/2_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 3 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/3_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/3_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      ILRMA <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/ilrma_est_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/ilrma_est_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      FastMNMF <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/fast_source_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/fast_source_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      Exterior Field Reference <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/1order/estFede1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/2_position/8_array/120/1order/estFede2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
  </tr> 
</table>

<!-- THIRD EXAMPLE -->
<table style="width: 100%; table-layout: fixed; word-wrap: normal;">
  <!-- SETUP -->
  <tr> 
    <th colspan="8" style="text-align:center;">EXAMPLE 2: 16 HOMs, 2 Female sources Mixture <audio controls><source src="examples/exs1/2source/3_position/16_array/60/mix_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio></th>
  </tr>
  <tr>
    <td>
      Source position: 3 <br>
      T60: 0.6[s]<br>
    </td>
    <td>
      Estimated Exterior field (input of MNMF algorithms)
      <audio controls>
        <source src="examples/exs1/3_position/16_array/60/input_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 1 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/1_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/1_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 2 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/2_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/2_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 3 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/3_order/est1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/3_order/est2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      ILRMA <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/ilrma_est_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/ilrma_est_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      FastMNMF <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/fast_source_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/fast_source_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      Exterior Field Reference <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2source/3_position/16_array/60/1order/estFede1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/3_position/16_array/60/1order/estFede2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
  </tr> 
</table>
