Docker Multi Container hosted on AWS - A tap to AWS

  <img src="data:image/png;base64,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U3nPMbj4DAEIQAACVN5TzgHEO+I95fym8p5jdPEZAhCAAASovCecA4h3xHvC6U3lPcfg4jMEIAABCFB5TzkHEO+I95Tzm8p7jtHFZwhAAAIQyLry/ve//9169eplM844Y5KZgHhHvCeZ2NNwSnnfLUfH8RkCEIAABJIgsJGZjezAEy/i/ccff7Tpp59+KjNmnXVWW2+99ey8886zxRZbrFTYEyZMsOuvv9522GEHm3nmmX927iFDhtjFF19sr7/+uvvd1ltvbYMGDbJlllmmVDtCnwzxXl3xPnHiRHdTedVVV9nuu+/uHLn22mutX79+9vDDD9u6667rfnbiiSfasGHD7N1336073VZffXU74YQTbIsttqj7mCrtiHivUrSwFQIQgAAEWhP42sxUVh5gZoPawONVvN9yyy0touPzzz934mGRRRaxBx54oNTIffHFFzb33HPbxx9/bPPPP/9U537sscdsnXXWcWNKAL3yyit2/PHH25gxY+yZZ54p1Y7QJ0O8V1e8y/KNN97YFlpoIbviiiucI7vssosT6hLsAwZoSputv/76ttRSS9mll15ad7qtssoq7vgtt9yy7mOqtCPivUrRwlYIQAACEGhNoJ+ZDTEzlb0nm9nAViLeq3i///777Te/+U2LjSeddJJdfvnlpvYVbddcc42de+659q9//ct23nlnJ6pVsX/hhRfstNNOs0cffdRWW201O+qoo5wA13brrbfasccea1999ZVtv/32duaZZ9qmm25qDz30kK244oqmMeeZZ56WMTWGKpkS+HPOOaf7+V//+le7+eabXTWyPTskCNZcc03bd9997eyzz7YNN9zQpptuOjvnnHPcMa+99po774gRI2z8+PF28MEHOxt+9atf2RlnnGG9e/e20aNH26mnnmprrLGGE2EvvfRSUzMW8V5t8a68ueyyy1xVXU+vlK+qvD/99NPuRrOozg8fPtw9Zbrrrrvs6KOPdvNpgw02sIsuusgWXHBB23///d1TpTvuuMMdf/7557eId+WhxtCTqnnnndfNAd1kzzHHHHbkkUe682rs2tzXeZZccsmm5m4jJ0e8N0KPYyEAAQhAIAYC/zSznlMMmVAj4geb2cTJk6Xpm7sVbTMS2n369NFbsk4w77nnnk7Mq4Xl3nvvtc0228wuuOACW3bZZZ0Q3muvvZyYWHrppV2Ljf5+4403un1fffVVJ5hXWGEFd4zEhASzBL/62DfZZBO7/fbbbfPNN7cZZpihxcG3337bVSr15/e//72rvkuYFH3v7dlxzDHHWPfu3U3tPkcccYQtvvji7gbju+++c605J598so0cOdK1NEicS/z88Y9/dBV+teR8+eWXrsqv8TS2hJH8b+aGeK+2eH/qqadcbuqp0EcffWQrr7yyffjhh64aP3bsWPvggw9s1VVXdb/7+uuvbfnll7dDDjnECW7lo25odcOrG81Ro0bZ3nvv7XJXv1fl/YcffrBtt93W5a326d+/vxPuumn4/vvvndB/8MEHbe21154q9zXPZp999mambkPnRrw3hI+DIQABCECgTgKj9AS8zn3L2G2imQ03s34+xXtbhr/zzjtOCG+11VZOdBctAur1lYh48803nWCXsNdF+c4773TtA+PGjbOBAwfa448/bo888og7tarsEjfbbLNNu20z2k+iX+dXtV3CR4JcVcpdd921XTt0jMT71VdfbbvttpsTN7PMMovdc889rtIv4XTYYYfZSiut5ATV+++/71qCxHe++eZzNyjyT+JdNxBLLLFEGXHs8ByI92qL96KyrhxT/j3xxBPuhlRPc3RT+9lnn9ngwYNdZV43lxLaTz75pHNaN8e6Cf7b3/7mboQl+JW72tQ2oydBV155pd122232u9/9zn766Sf3JOm6665zN6XaNB90E6qnS7W53/TEbXAAxHuDADkcAhCAAATqIqDyd7M+kNC68i6D1D6jyvsEn+JdVb2i8i6RrUf7qn5fcsklrrr+1ltvTQVLovqbb75xwldCXRVIvdz63nvvOfGuyqAE8YUXXjjVcR31vKslR604M800kztGokjtOxLyEkNqx2nLDp1TAkYvuUoUaZMo0nkk2lVNVx+/Ku19+/b9WdDlowS+ngTIJx8b4r3a4l3W66ZVrWIS5b/97W9d25Yq5Kq0K4/mmmsul/9qGVtggQVa2rg0P/RE6LnnnnNPgFRt15OrQryrFU2b2tRUrf/HP/7hjm+9KZfVUtM6933kb1fHQLx3lRzHQQACEIBAZwg0S7zX9rwXov30GsOC9rxLhOgFUv1Re4CEfdF3rjaTTz/91FX+VKUeOnSoE8US1qo8Spyov10iRD242p599llXSdd52nthVVV7tdGo6lhsaj9YdNFFndA54IAD2rRDY0rA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RRe15557zp566ilbbLHF7N13301jmnr0AvHuETZDQaB8AsEucuW7EvUZ4Rx1eJI3Lrf8C+ZvFuL96aeftl//+te25ZZb2l133WXLL7+8vf76624Wvfrqq/bBBx/YFlts4YS9BP4tt9zi/vvRRx+56vwFF1zgqvGFeD/mmGPsvvvus0mTJtkhhxzibgZab0Xl/Z577rFNN93U7TvXXHPZt99+a2PHjrVvvvnGne/JJ590gv6//uu/TOft3r27s03Hy7b999/fXn75Zffz4cOHu2OPOOIIu/fee23BBRe0vffe2/bZZ5/kVwTEe/IhxsG0CQS7yKWN9WfewTmzgEfmbm75F8zfLMR7IZyV5P/4xz9s1llnde0rF198sV133XWuXebkk0+2kSNH2swzz2xrrbWW22eVVVZxrTZLLbWUE9QSzaq8a1PbjES1trffftuWWGKJqeZQa/Guanuxz9dff2077bST/fnPfzZV5nW8bLj66qttt912a7m50JOA4iajqNhvvPHGzk7djLz33ns2ZswYJ+p32GGHyOZwueYg3svlydkg4JlAsIucZz9DDwfn0BHIe/zc8i+Yv1mId80l9ZvffPPNTiCrUi5Rvt5667nq9+jRo93fv/vuO1dJv/zyy23YsGG2/vrr25577umq3I899pjdeuutTryrZ17iv+idL/5eO2cL8a6bgB49ejiRrU2V8ksvvdTOOOMMm2222VzFXZV9nffEE0+0PfbYwxZaaCHbeuut7Y477rAnnnjC3UxIvI8aNcoWWWQRd+MgmyTsN9poI/dnxIgRSS8ZiPekw4tz6RMIdpFLH+1UHsI5s4BH5m5u+RfM32zEu3rcJdpVsVbv+VdffWXbbLONE+zPPvusbbLJJq4V5je/+Y0Tya23G264wZ555hknsl944QXr3bu3+6+q86qiX3/99W1W3lW1n2eeeWzhhRd2rTmbbbaZzT777HbllVe6Gwe10RSbxLteZt1xxx3trLPOcpX+H3/80aaffnon3ocOHeraeFpvOfTRI94jW6IxBwKdIxDsItc5Myu390ZmdquZHWRmQ82s4NzPzM43s75mlnZlp3IhS9rg1Od5NPMtG/H+4YcfOgGtrRC7/fv3dxVwbeeee66ruks433jjjU4or7baajZu3DgbP368a53Ri68S76rgb7fddq43vm/fvi1Cu63Ke9Hz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4CRe874BOzt1aCHeNc969OjRcqxuNvV06LLLLnPrd1s5pp1vvfVWtzYrPzfYYAOXf5qHV155pTvu2GOPrWuudMroADsj3gNAZ8guE9CFeQYzO6JGtBcNm2PMbN4un5kDawmUKnZ8oZV410ItgSTR8OSTT7pKem3lXT9feeWVbauttrIzzzzTnnrqKXvjjTfso48+ammbOfHEE+2kk06ygQMHOoG1//77uz8SZTpeIuawww5z//+Xv/zFNt54Y18uljJOQLHTLPEuLv80s55TAE2oEfGDzWyiLt5lbYV4V34sueSSLacV1x122ME9wZHIkCBXpe/II490P3v44YedkN9rr71ce5fyTzd9d9xxhxO1xx13nG2yySZ21FFHOQG82WabOZG+7LLLOmGs4/bbbz93cyqxLfF9+OGHu6dNOl9bP1ee1m5vv/22LbXUUu6P5oUEkfK56Hu/99572xxX1c7u3bu7p1pHHHGELb744u6G4rvvvnMtRCeffLKNHDnS+ShxPsccc7j5ohteteToyZaqpxpPY4vJnnvuWUpIAuZzKfY3eBJved+gnXUfXoj3Dz/80In3H374wZ5++mn77W9/6256+/bt226Off3117bIIou4Ao1ulpVneqqk+a91XTfIuuGsZ67UbXCgHRHvgcAzbJcI6Ao83My2nSLiu3QSDpo2gTLFzrRHK2ePQryrCijRIuGg6qTEjdpmJMAlxseOHWszzDCDaxOQ0GhLvD/44IP2yCOPOMMkXPQIV5XUxx9/3NZee21TD6ZEu6o5VdumiJ2qmd0VeydOWS/6lZnPhXhfbLHFnEgtNlX6itYTCdbiHQv1mO+yyy5OeEi8S5hLLKs6r7yUAFaFXUL9k08+cYJeN5dqwbniiivc6a+66ip3YyqBrPc3LrzwQvdehyro6sGXyGnr56rqt940P3Q+3QDoplWCXNV73QC0N66OkXgv3icpGNxzzz226aab2vLLL+/m3EorreSeMkgkSUSJ+3zzzed67OWPxLtuIJZYYomuxLPNYzLK53qZNSXv6x280f3a6nnXObV2v/DCC6ZWmPZy7JtvvrHzzjuv5amO8vrAAw+cSryfcsopdc+VRn1p5vGI92bS5dxlEygq70dOqbzr71Tey6ZsWuvKq1SWb17bZ6wV76rAqMKnVoAnnnjCiSQt/lrYJei16SsEEiRtiXdVfSRUtEk0qfKjlhptEu0SUYVA8eVfWeMkWqlsXYEULrXPqPI+ocx8nlbbjAYu9tFNnnJJzCXe9Ti/aBf56aef3KN9PSHSjaZeINUNojaJ7rfeemuqkEtkS5yozUvVb22bb765E/56AtDez2tPohYctd6ol1ibRLmeMknIq3VMLwq2Na5uEjRXZKOeBGjT0wCdR6Jdc+3zzz93fqgy2npTC5sEvuyVD2VukeVzM58utYXNW96XGbOOzlXb866bUq3To0aNck969FRVc6a9HFNxRTfUurnVpnVbT19rK++6TtQzV3z529VxEO9dJcdxIQi0Xhj15op63vVzet7Li0jlxbtQaKHfZ599bMUVV3SiRFVBtR7oEb4uAKpyzj///G2Kd/UeF1XPWvH+7LPP2uqrr+6qlap8qlpatS0ysVMGvtre30K0176dXGo+1yPedZOoG8dvv/3W9eBuu+22TrzrMb4q7trUay4h/O6777pcrRXvamXp06dPSx+6clb9uqpm6/9/+ctfuptStQLo/5WHbf28uBkoIOsJgJ461T4x0hc4Fl10UXvuuefsgAMOaHNctYgVN7rFV2nuu+8+91RLrTtqP9PNrXre1fojWzVHtMkvPRWQv4j3MtK95Rxe875Uyzs4WXs972qD0ZMhzY32ckxPePRuhVrRtCn/JfprxbtuduuZK7787eo4iPeukuO4EATaq2oUIp6vzZQTlVLFTjkmTfsstZV37a0FWwLo0Ucftf79+9see+zhKpR6GXD77be3o48+2r3U2lblvS3xLvGlF+/UNqPPAerrB7rQrLXWWtM2LqI9EhTv+uqGSsn62kxbnxQqNZ8L8a5Pk+rGsHbTzaCe+qgt5IYbbnCCVS+lKsckbNU2o1YT5aVy8qabbnIvqeoGsVa86+VUVcO1r0Tw3nvv7VpjJP7XW28996K02nYk3vUkSdXztn7+v//7v1PZJ9GuXnNVyLW/+ok1ts6jirj68NsaV762Fu86Vl90qr1BUUua+on1ST/1HesJ1RZbbOFaHVS9R7yXuhB4zftSLe+CeNfL2XrXQut2ezmmFjK9pHrnnXe6jxbstNNOLgdrxfshhxxS11zx5W9Xx0G8d5Ucx4UgMK1HktP67m0Im6s4ZqlixxeA1uJd4xafCpNQUstC0brw8ssvu0evEirvvPOOa4EpvvMuIdNavKvirsqPzlF8hlKVd7U86EU8VTOrsiUo3vXG8IgO+Jeazx195109thIOErZ61K/+9v/4j/+w9ddf332hpRDheolOLTX6ipHEhvrjJfAlkrV99dVXrlqvc2jTV21UwVf7l/L2lltucT3kahFQe9d//ud/tvvzWi4//vijE9WqUBabXuDWy7cS2e2Nq5sSiXfdjNT20aufWD4XL67qnLoh0Yu7xSbfJLh0o6uXcGmbKW2l8Jr3pVk9jRMVlXfNs6K9S4foplOFmOLrSG3lmFrRND/0RTBt+jcMNB8L8a53l/Q1pfbmkC8fyxgH8V4GRc7hi8C0xLsvO1Ifp1SxEwssPSqVGFIFRyJGPb4SQxJaKf4LfO1xT1C8TyvFoshn3TjqSxe64StaVTr6xKgEh8SGvlijnvLaFzP184kTJ071tRtBaO/nrQFpLsgGteEUn4ws9ulo3GmBLn4vMa+b3AUWWOBn56/3HPXuF1k+x3SNiiLv641jZ/frKMeU2xL+elm6va3eudJZu3ztj3j3RZpxyiAQ08JYhj+xniPJRV8vPumlOfWsq9VFX9zQo9UqfjGmkcSJTOw04kq9x0aRz4V4r+o/hlQvbN/7RZbPMV2josh73/mQy3iI91winYafMS2MaRBt24tkF31VZO6++27XKqP+db3MlFPVXeGOTOz4mEdR5LN62iXc1W7FVh6ByPI5pmtUFHlfXqQ5Uy0BxDv5UCUCMS2MVeLWWVtZ9DtLrEL7RyZ2fJAjn31QDjRGZPkc0zWKvA+Ukz6GRbz7oMwYZRGIaWEsy6cYz8OiH2NUSrIpMrFTklcdnoZ89kE50BiR5XNM1yjyPlBO+hgW8e6DMmOURSCmhbEsn2I8D4t+jFEpyabIxE5JXiHefYCMcYzI8jmmaxTreIwJW5JNiPeSQHIaLwRiWhi9OBxoEBb9QOB9DBuZ2PHhMvnsg3KgMSLL55iuUeR9oJz0MSzi3QdlxiiLQEwLY1k+xXgeFv0Yo1KSTZGJnZK8ovLuA2SMY0SWzzFdo1jHY0zYkmxCvJcEktN4IRDTwujF4UCDsOgHAu9j2MjEjg+XyWcflAONEVk+x3SNIu8D5aSPYRHvPigzRlkEYloYy/IpxvOw6McYlZJsikzslOQVlXcfIGMcI7J8jukaxToeY8KWZBPivSSQnMYLgZgWRi8OBxqERT8QeB/DRiZ2fLhMPvugHGiMyPI5pmsUeR8oJ30Mi3j3QZkxyiIQ08JYlk8xnodFP8aolGRTZGKnJK+ovPsAGeMYkeVzTNco1vEYE7YkmxDvJYHkNF4IxLQwenE40CAs+oHA+xg2MrHjw2Xy2QflQGNEls8xXaPI+0A56WNYxLsPyoxRFoGYFsayfIrxPCz6MUalJJsiEzsleUXl3QfIGMeILJ9jukaxjseYsCXZhHgvCSSn8UIgpoXRi8OBBmHRDwTex7CRiR0fLpPPPigHGiOyfI7pGkXeB8pJH8Mi3n1QZoyyCMS0MJblU4znYdGPMSol2RSZ2CnJKyrvPkDGOEZk+RzTNYp1PMaELckmxHtJIDmNFwIxLYxeHA40CIt+IPA+ho1M7PhwmXz2QTnQGJHlc0zXKPI+UE76GBbx7oMyY5RFIKaFsSyfYjwPi36MUSnJpsjETkleUXn3ATLGMSLL55iuUazjMSZsSTYh3ksCyWm8EIhpYfTicKBBWPQDgfcxbGRix4fL5LMPyoHGiCyfY7pGkfeBctLHsIh3H5QZoywCMS2MZfkU43lY9GOMSkk2RSZ2SvKKyrsPkDGOEVk+x3SNYh2PMWFLsgnxXhJITuOFQEwLoxeHAw3Coh8IvI9hIxM7Plwmn31QDjRGZPkc0zWKvA+Ukz6GRbz7oMwYZRGIaWEsy6cYz8OiH2NUSrIpMrFTkldU3n2AjHGMyPI5pmsU63iMCVuSTYj3kkByGi8EYloYvTgcaBAW/UDgfQwbmdjx4TL57INyoDEiy+eYrlHkfaCc9DEs4t0HZcYoi0BMC2NZPsV4Hhb9GKNSkk2RiZ2SvKLy7gNkjGNEls8xXaNYx2NM2JJsQryXBJLTeCEQ08LoxeFAg7DoBwLvY9jIxI4Pl8lnH5QDjRFZPsd0jSLvA+Wkj2ER7z4oM0ZZBGJaGMvyKcbziDNb2gS6pe3eVN6Rz+kHO5Z8jukaRd4nnvdK+pgSLnHcuNcAAfK0AXgcCgEIQAACTSXANaqpeDl5LQHEO/lQFQIsjFWJFHZCAAIQyI8A16j8Yh7MY8R7MPQM3EkCLIydBMbuEIAABCDgjQDXKG+oGQjxTg5UhQALY1UihZ0QgAAE8iPANSq/mAfzGPEeDD0Dd5IAC2MngbE7BCAAAQh4I8A1yhtqBkK8kwNVIcDCWJVIYScEIACB/Ahwjcov5sE8RrwHQ8/AnSTAwthJYOwOAQhAAALeCHCN8oaagRDv5EBVCLAwViVS2AkBCEAgPwJco/KLeTCPEe/B0DNwJwmwMHYSGLtDAAIQgIA3AlyjvKFmIMQ7OVAVAiyMVYkUdkIAAhDIjwDXqPxiHsxjxHsw9AzcSQIsjJ0Exu4QgAAEIOCNANcob6gZCPFODlSFAAtjVSKFnRCAAATyI8A1Kr+YB/MY8R4MPQN3kgALYyeBsTsEIAABCHgjwDXKG2oGQryTA1UhwMJYlUhhJwQgAIH8CHCNyi/mwTxGvAdDz8CdJMDC2Elg7A4BCEAAAt4IcI3yhpqBEO/kQFUIsDBWJVLYCQEIQCA/Alyj8ot5MI8R78HQM3AnCbAwdhIYu0MAAhCAgDcCXKO8oWYgxDs5UBUCLIxViRR2QgACEMiPANeo/GIezGPEezD0DNxJAiyMnQTG7hCAAAQg4I0A1yhvqBlI4n2Uma0PCghETuBBM9sgchsxDwIQgAAE8iSAeM8z7kG8lnhngwAEIAABCEAAAhDoOgHEe9fZcWQnCSDeOwmM3SEAAQhAAAIQgEArAoh3UsIbAcS7N9QMBAEIQAACEIBAogQQ74kGNka3EO8xRgWbIAABCEAAAhCoEgHEe5WiVXFbEe8VDyDmQwACEIAABCAQnADiPXgI8jEA8Z5PrPEUAhCAAAQgAIHmEEC8N4crZ22DAOKdtIAABCAAAQhAAAKNEUC8N8aPoztBAPHeCVjsCgEIQAACEIAABNoggHgnLbwRQLx7Q81AEIAABCAAAQgkSgDxnmhgY3QL8R5jVLAJAhCAAAQgAIEqEUC8VylaFbcV8V7xAGI+BCAAAQhAAALBCSDeg4cgHwMQ7/nEGk8hAAEIQAACEGgOAcR7c7hy1jYIIN5JCwhAAAIQgAAEINAYAcR7Y/w4uhMEEO+dgMWuEIAABCAAAQhAoA0CiHfSwhsBxLs31AwEAQhAAAIQgECiBBDviQY2RrcQ7zFGBZsgAAEIQAACEKgSAcR7laJVcVsR7xUPIOZDAAIQgAAEIBCcAOI9eAjyMQDxnk+s8RQCEIAABCAAgeYQQLw3hytnbYMA4p20gAAEIAABCEAAAo0RQLw3xo+jO0EA8d4JWOwKAQhAAAIQgAAE2iAQk3iXLWwJE0C8JxxcXIMABCAAAQhAwAuBqMT75Mnody9RDzBIt27dDPEeADxDQgACEIAABCCQFAHEe1LhjNcZxHu8scEyCEAAAhCAAASqQwDxXp1YVdpSxHulw4fxEIAABCAAAQhEQgDxHkkgUjcD8Z56hPEPAhCAAAQgAAEfBBDvPigzhiHeSQIIQAACEIAABCDQOAHEe+MMOUMdBBDvdUBiFwhAAAIQgAAEIDANAoh3UsQLAcS7F8wMAgEIQAACEIBA4gQQ74kHOBb3EO+xRAI7IAABCEAAAhCoMgHEe5WjVyHbEe8VChamQgACEIAABCAQLQHEe7ShScswxHta8cQbCEAAAhCAAATCEEC8h+Ge3aiI9+xCjsMQgAAEIAABCDSBAOK9CVA55c8JIN7JCghAAAIQgAAEINA4AcR74ww5Qx0EEO91QGIXCEAAAhCAAAQgMA0CiHdSxAsBxLsXzAwCAQhAAAIQgEDiBBDviQc4FvcQ77FEAjsgAAEIQAACEKgyAcR7laNXIdsR7xUKFqZCAAIQgAAEIBAtAcR7tKFJyzDEe1rxxBsIQAACEIAABMIQQLyH4Z7dqIj37EKOwxCAAAQgAAEINIEA4r0JUDnlzwkg3skKCEAAAhCAAAQg0DgBxHvjDDlDHQQQ73VAYhcIQAACEIAABCAwDQKId1LECwHEuxfMDAIBCEAAAhCAQOIEEO+JBzgW9xDvsUQCOyAAAQhAAAIQqDIBxHuVo1ch2xHvFQoWpkIAAhCAAAQgEC0BxHu0oUnLMMR7WvHEGwhAAAIQgAAEwhBAvIfhnt2oiPfsQo7DEIAABCAAAQg0gYBP8b6RmY3swIfJkyfLnHi2tdde2x5//PEWgxZccEHbbbfdrH///jbLLLN02tAJEybY9ddfbzvssIPNPPPMnT6+ygcg3qscPWyHAAQgAAEIQCAWAj7F+9dmNqOZDTCzQW0AiFK8r7vuunbIIYeYbizefPNN69Onj11xxRW2xx57dDqGX3zxhc0999z28ccf2/zzz9/p46t8AOK9ytHDdghAAAIQgAAEYiHgU7z3M7MhZja9mWncga1EfJTiffPNN7ejjz66JV7//d//7f7/1ltvtTfeeMP2228/e/75522ZZZaxc88919Zaay33+zPOOMOuuuoq+/77722fffaxY4891jbYYAN76KGHbMUVV7T777/fxowZYwcddJB9+umntvPOO9vo0aNt8ODBNnbsWDv11FNtjTXWsGHDhtlLL71kzzzzjB1xxBHuBmKTTTZxY+lG4Msvv7QBAwbYjTfeaD179rRBgwbZlltuGUt+tdiBeI8uJBgEAQhAAAIQgEAFCfgU78LzTzPrOYXThBoRP9jMJsbYNrPRRhvZkUceaT/++KO98MILThhLYO+66662xBJL2AorrGDHHHOM/eUvf7Hzzz/f3nnnHXv//fdtq622sjvvvNM++OAD23vvvZ1Y/+qrr5zwvv322003BauttpqtvPLKbt8zzzzTnnrqKXdD8M9//tNU8V9qqaXc2BpzvvnmswMPPNB086B9v/nmG3vkkUfs7LPPdueW2L/vvvvsuOOOs/Hjx9uMM+ohRzwb4j2eWGAJBCAAAQhAAALVJTDKzNYPbP5EMxtuZv1iFO+1Pe/itO+++zqh/PTTT9umm27qRPSss87qEM4222x26aWX2vTTT299+/a1Bx54wInw119/3eaZZx4nqIu2mZ9++smWW245V2WfYYYZXGVdlfZa8f7222+7G4TzzjvP3TB8+OGHJhGs6rsq/Z988omdfPLJTvQPHTrUll9+edejrxuC2HrqEe+BZxnDQwACEIAABCAAgS4QaF151ynUPqPK+4QYxbsEtVpjtPXq1atFqEukX3DBBfbaa6+1YNALrqqMq0KunngJagn73Xff3U4//XRXES/Eu4S9RLlabrRNmjTJunfv3iLeVZnXjYE2ne+iiy76Ge5XXnnF5phjDvcCrET7YostZoceeqgdcMABXQhNcw9BvDeXL2eHAAQgAAEIQAACZROo7XkvRPvpNYNUoue9sFctK1tssYXrOZ9uuuncC62zzz67a11ZYIEFXJVdf9TSIjF9yimn2Lbbbtsi3h999FHba6+9Wo5XFV0vsRaV91rxfvzxx7u2HPXLa/vhhx/s1VdfdW03b731li266KL2+eefuzYd9dCr0r/sssuWHb+Gzod4bwgfB0MAAhCAAAQgAAHvBPS1mZmmfG2mVrQXhlRKvEtAq4p+1llnuSr7yJEjbfvttzd9UWbIkCF277332vDhw52gX2+99Wy77bazXXbZxeacc04nvCXsl1xySddmo+P0Uuwll1zSpngfMWKE65V/+OGHnWDXmBpDX61RpV8vwErgf/vtt84m9eb37t3be4A7GhDxHlU4MAYCEIAABCAAAQhMk8DGZjaig70qJd7lhwS0qupqjZFwvvLKK+0Pf/iDffbZZ7bqqqvaRx995H4ncX3XXXfZXHPNZcW34yW8Vb1XO83LL7/seuRvvvlm98KrqvCbbbZZS9uMxjr88MPtnHPOcfjUvqMbA3295sEHH3T/LfrudR59yjK2DfEeW0SwBwIQgAAEIAABCDRGIDrxXo87+oKMRLr6zWtfEtU/yPTee++5Sru+FFO7qdVG26hRo2ybbbZxX7KR4F9ooYVcS4xeeG1r01dotJ9eYp1pJj3E+L9NvfH6qs3iiy/epX88qh4/G90H8d4oQY6HAAQgAAEIQAACcRGopHjvKkK9oKqvw6y++uru2/D6Jrw+O6nqfYob4j3FqOITBCAAAQhAAAI5E8hKvCvQqpbffffdrlVGPer6h5raq7pXPTEQ71WPIPZDAAIQgAAEIACBqQlkJ95zSgDEe07RxlcIQAACEIAABHIggHhPOMqI94SDi2sQgAAEIAABCGRJAPGecNgR7wkHF9cgAAEIQAACEMiSAOI94bAj3hMOLq5BAAIQgAAEIJAlAcR7wmFHvCccXFyDAAQgAAEIQCBLAoj3hMOOeE84uLgGAQhAAAIQgECWBBDvCYcd8Z5wcHENAhCAAAQgAIEsCSDeEw474j3h4OIaBCAAAQhAAAJZEkC8Jxx2xHvCwcU1CEAAAhCAAASyJIB4TzjsiPeEg4trEIAABCAAAQhkSQDxnnDYEe8JBxfXIAABCEAAAhDIkgDiPeGwI94TDi6uQQACEIAABCCQJQHEe8JhR7wnHFxcgwAEIAABCEAgSwKI94TDjnhPOLi4BgEIQAACEIBAlgQQ7wmHHfGecHBxDQIQgAAEIACBLAkg3hMOO+I94eDiGgQgAAEIQAACWRJAvCccdsR7wsHFNQhAAAIQgAAEsiSAeE847Ij3hIOLaxCAAAQgAAEIZEkA8Z5w2BHvCQcX1yAAAQhAAAIQyJIA4j3hsCPeEw4urkEAAhCAAAQgkCUBxHvCYUe8JxxcXIMABCAAAQhAIEsCiPeEw454Tzi4uAYBCEAAAhCAQJYEJmfpdUZO/38/FWuoWcvQ+gAAAABJRU5ErkJggg==" style="cursor:pointer;max-width:100%;" onclick="(function(img){if(img.wnd!=null&&!img.wnd.closed){img.wnd.focus();}else{var r=function(evt){if(evt.data=='ready'&&evt.source==img.wnd){img.wnd.postMessage(decodeURIComponent(img.getAttribute('src')),'*');window.removeEventListener('message',r);}};window.addEventListener('message',r);img.wnd=window.open('https://www.draw.io/?client=1&lightbox=1&edit=_blank');}})(this);"/>

