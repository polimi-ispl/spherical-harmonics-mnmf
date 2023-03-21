In the context of source separation solutions for virtual reality (VR) applications, several techniques in the spherical harmonic domain (SH) have been proposed in the literature. The performance of such methods is limited under high reverberation conditions and the rendering of the obtained spatial sound is fixed to the recording location only. Recently, novel sound field works in the literature proposed a global representation that enables both the estimation of the direct sound (exterior field) and the reconstruction in locations different from the acquisition ones. In this paper, we propose a signal processing framework based on Multichannel Non-Negative Matrix Factorization (MNMF) in the SH domain that operates directly over the exterior field coefficients enabling the reconstruction of the direct sound field of the separated sources. To evaluate our proposal, we compared with other state-of-the-art source separation approaches using several setups and including different reverberation conditions, showing promising results in terms of SDR metrics.

### Method
<!--  ![Image](figures/pipeline.png) -->

# Listening tests
Audio examples will be available soon.
<!--- Here below we report some audio examples along with the spectrogram of the signals. <br>
For each example [...]. <br>
We compare the results of the proposed method with the FastMNMF and ILRMA.
--->

<table style="width: 100%; table-layout: fixed; word-wrap: normal;">
  <!-- SETUP -->
  <tr> 
    <th colspan="4" style="text-align:center;">EXAMPLE 1: 4 HOMs, 2 Female sources</th>
  </tr>
  <tr>
    <td>
      Source: 1 <br>
      T60: 0.3[s]<br>
    </td>
<!--     <td>
      Mixture
      <audio controls>
        <source src="examples/exs1/2_source/4_array/30/1_order/.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    <\td> -->
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 1 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2_source/1_position/4_array/30/1_order/est_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2_source/1_position/4_array/30/1_order/est_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
    <td>
      <!-- <img src="examples/exs1/ds1/mixture_mic0.png" title="mic0" width="100%"/> -->
      Sph order: 2 <br>
      Source 1
      <audio controls>
        <source src="examples/exs1/2_source/1_position/4_array/30/2_order/est_1_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio><br>
      Source 2
      <audio controls>
        <source src="examples/exs1/2_source/1_position/4_array/30/2_order/est_2_mono.wav" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </td>
  </tr> 
</table>
