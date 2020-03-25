<template>
  <div class="ud">
    <title>Unstoppable Domains</title>

    <Navbar />
    <pricec />

    <br />

    <h2
      class="display-4"
      id="title"
    >

      Unstoppable Domains

    </h2>
    <section>
      <br>

      <h1>What are blockchain domains?</h1>
      <b-container class="frame">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/Zm6uZzZwLSg"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </b-container>
    </section>

    <br>
    <b-container>
      <h1 class="display-4">Overview</h1>
      <udcara />
    </b-container>
    <br>

    <section class="list1">
      <h1 class="display-4">Features</h1>
      <br />
      <ul id="example-1">
        <li
          class="display-4"
          v-for="item in items"
          :key="item.message"
        >
          {{ item.message }}
        </li>
      </ul>

    </section>
    <br>

    <section class="integrations">
      <h1 class="display-4">Integrations</h1>

      <b-container>
        <b-row>

          <b-col>

            <li>
              <h3>Coinomi</h3>
            </li>
            <a href="https://www.coinomi.com/en/">
              <img
                alt="Coinomi"
                src="https://99bitcoins.com/wp-content/uploads/2018/06/coinomi_logo_compear.png"
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>Atomic</li>
            </h3>

            <a href="https://atomicwallet.io/">
              <img
                alt="Atomic"
                src="https://unstoppabledomains.com/_next/static/images/atomic-logo-387374d0f0e665c037cdea5a7436c2b3.png.webp"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>Moonlet</li>
            </h3>
            <a href="https://moonlet.xyz/">
              <img
                alt="Moonlet"
                src="data:image/webp;base64,UklGRgIUAABXRUJQVlA4WAoAAAAQAAAAxwAAxwAAQUxQSDMKAAABoMb/1+qmOWmSumJ1pBR3m+DuMDd8vuHu7i5zwbUw7Qx3qBfX0nU1HOqSNk3Oi957cp/0PPflPhExAfA/SU0e3m4G3Vejx9gtv569dGzX3G7eOs6v96aEp6j69HBfvdZ02pkipOet99VjkTNvoYZL3XRX6Lx/UdPS6TrL+PY11Do1Qld1PlCE2s/XUX6TM1FkYqhuanUYxZa8q5NcJ2Wh6I36qOHWUhR+3EMP9buCTnivuv5x+fwhOuOj+roncL0NnfJ5K73T5DCSy9MTY2LiMzUp7qZz+l1FoiVx6ZAmPmZXz6Zj4jUo6aFvXv0P1R8fGBbuAqoRWyocKtY1pqmFqPrgu9ZAd1ludaREz5hmWlC5JLqbARz1iXIkp61+CdxWjor24wPcQMOIuw48aaxbvLaicv7yQNB2gwP3w/VK/Wi70rkhoHWnZ7Q7/jol8DAq2nYFgua+f9LOeumTJkdQ8cEHXiBwpp20x6RLGl5ExZhOILTrI9JS0KMtz6LiwXogttZVSsUHeqRhHFa2flcdBJsOUx711CFNErGyZY4RhH9LSa6nP4IOY+VHH4ATLqJEG3WCuUajdt0HvfXG8AmT/8LKFV9G+hvFTaCsBumbQtq+OXf7qeTUhwVWpNqy7iWd2D73zXZ1zCKGEexvy80U3H3atgtPbCiwIidp55x+Ya5avU141lpipvZzf04rRqcszfpzSXd3QTHVZGVqPjY6FZ0688iMl71E7AY5h488lIlVMOfI1JYGrUo+k1LEjBgbVtXULzqatElvJaHGC1KxSucfHOxG+FAtOkA6IfNSsMrn/TTIoDJFbRZI1md4ArKYv/UlpaUqZX0l03yvBbnMnh5Y6RuV9DCpVF+ShZxeHeYGpt9VfjTKpGk0Mlv6XTWIUbIPA3kaRqYgv8fH3FZKaSAPr9kFyHGhRWmvURrB22zIufUtkGXds8h7apAs6hxB5neCJNucRuaL3pNExGnk/lptOTQ4j+yvACkG/IHs53STgsd25P+ouxSmlUtgNshwcDHyn95BBpGxKMGvXCVg2o0StPQHCb5TLIO4mkqm9u58tbiGErRPBOWapz9my2UryvBBE5WORbdqctW9UAp7zSrjEKcx5XMIZVgwFJT9DiH+15Knt4qkcMJPpe1/iLjBwJHfUZTiOFCdUIaID9px9F6ZFG5FqkVh5U0Muf6GUlwEqkGpCimt+Bn0RAoZrdXesCjYVrFj2IVS/ApUjXtR+UYgN5HZUrD0VaufomIdyc0slOJRb7VRNhX8xciLx1EpWEaCqutvqJ4eyUurZ1I45afWOp9gH8fLRLsM7J+B+nikRrtx4nkSZXglQK36CVJ2M06aZcugYjaoD8gn2V7n5M0KGSRHqBl3In0JJwtRhrNAvWm6A38a+XD5WQYpEYSx6ODNMD5qXpbBSlD3/NuR50P46HJfAtcaE4blOGKfyccHpRKYBurGn9Dh7wxsLEX+sxsR2jx07E9/Lsw7JLAGiBvR8cu1ufD/i7+MFoTgmxo8asZFeCJ/S4H4uU2Doo5cRKawl9GIUOMcalg6iIuWz9lbA8R3K7SwjuaiTT5315oQzL+jlvbxXPQsZs46Foiv5msziYshpcwlBBO8f0Ztl3MxmDn7Z0AcUKzRen2UHELZgzqu7C0gtn2m1TouBvF20otg3IRaz+aiQwFneYOA2OWJVvbxXLTO52yfibIdtbZ9zkXjDMayOwHxpRzNLK9xUfcaY5uA6Po9al7cg4taZ/i614Yy+Kl2ua258Ixiyz4RiO7/oPYpkVzARrZO1aC8UiLgVC02JtmYKh8KxFqnUeBedzaGPGfqb2/KhDIRy4HNiDs8ZfUEYtBVFFgymg/XkzytAeocm4iMDnzAFpau1aY0z0CRF70Y+YQjyzigbkGhW4HRTnkMHfSmdM8X8xkngdf5yesJRM+9KLSwKyeGLfwsB+rHFjHJNTmBvhZuEkIpEddR7CZgtdYVZgrfAOoqFFvYjRf4hpkoI6VNlqCEAGZ6FbJyqxUQvaNR8HJg1uscJ+WjgTrKLii3HTcw2cJIlAel8Q0U/JuZnTqX+Uh/EYiu36LgwmHA7xI2rJ8B9Y0iUX/7MtQ8nYvf3Sg1z6Poj4Dj9UyktQOiYaNVVFwIS5FXWSj5AKhvFqLg0tHA81gWDrhRqsWh6IO+TNVIZiC1BRCNy1F0YUfgepytypV+AtQhOcJ2mtiai1V+kwslPBFFJ9QHrj1OVLk7DYHoshpFl40Ctps+qWrPBgF1dIGwHWa+RmBVXwrURndR9PkIYNv166p23I/i+zuKzukKfNe7VslWVmXudQHqxHJR5bOA8dfKKmUvyKgiRcOA2uUpCratdeNsPVaO8x1bXDW+MVLCzqDogx7AeLWzCgfBMLGkKvwdBETPfSh6fwhw3vGZwgIAWGB1vqzWQB1XIeq36sD6GKxsGQoAHjMLnS13BFD7pqHgv5oB718q5DSCypPKnWwFUOvcRMG7/YF3r5MKd4IUTBOfOtWpmhSf/SjWticQmH8hVeGslwLAgBtOFNMMiMYNKLZgritw/7FF4VeDCrQ67DRP+wB1VIGYlGEmYH8zKm4FYuAPhc5hnQLULmkoNPZl4N/jmNJKCpiG33OKbV6Uhkko0rIxGCQYlKFQMZMEELm5WNxxPyD6RKPImNcMIMPOBQpFHzoA5jdPiUpuBUSPjVYB2avrgBzH2RQKRzkC4PtxrF1ERhegzrOj5k9+bAey3IyKOa85BhCy6p52xZ8C9e1i1NpycqgRZGn6XelhVy0AwqfE27WpmGykvPMENS6IGuAF8qweJwYgdNz5Ui1+cANihxTU9v6u3l4g03rpSrlvaAUQMGhDYpkD9kO1gPhyEmqZET2xhRHk2rpYqXCUdgAQNGJbhpVyqiYQGyaj47kn5nYwgnSHlCuVfi4EwFh3+P48lZvtgFj3JNKt+deiprbxBBlPtCnhMkEApiVFSqkdgVj3NKrbn10/snFUu0ADyNmwElV/EFV/pxUVn7wBRO9laSkpNxJiones+vz1rpEeIHGXHWpHXMX0SkDlgk+B6hnZsEHDMA93kwGkb/pL7W6QCP+FD1HZMhF0qmusWnE3Aa3/RNWimaBXzRfVcKNmftPTUNU636hbPOMJd+pp1Oc4qpevNoNuDb5JsM3TpOnaB6huXeYN+jXgEgHzejrWbHkmEi2zDaBjzRcpeKEZzdBsYQpSrUvMoGddaXh3hJ+KT9PPoh4iOX+WEXSt6U8aFv02umPzhh0Gjt2TWoH00llm0Lcu3ziAiDmZaY/L0OHHU1xA786yO6Tt01dB//Yvc4bb/UEHN3nqBBdeAD3sf0GYbV890Mdfi7Ks8gOdPKhETOq7RtDL3heEHG8LOvrDQu0eLw0BPe0WpVlMV9DZ7VO0ub8qFHR35ysa5H7dDPT4iydtDmTu6uMB+jzgkwv5ajnxS1oaQL/XHLTkUOzly+f2zOxXHfS+0dPb28MA/58UAFZQOCCoCQAA0C4AnQEqyADIAD6RSJ9LJaQjIaNVqfCwEglibvx8e0AZbcIP4vuSOJ9u/qXJlcY+LvWr33R5u2TQh/evUN5gH6x9IPzAecz/rv1u91n9g9QD+jf8XrCfQA/a703/ZC/rn/a/dj2y/UA//+wxf5b8E/DrIV3d9o3sHlLA32QjKH5CW1yjG9ePoqrmszMxHUUrnqsWWl82E550DMmCkwCfdAp+ru9GDn04CWJz4r5w284uX+QvNXMrlEGg78bp8y9ewMs7Tjcrd/VmYfvKTGIpNigh3Hwj8tfcVf57wvc2GZlQHe4pvnkPllVpSsfDut8c+EHFzJZa4b3PylmTtEAafDRQmkCWNd4mJygt53wlmWdpuZwrSGkJM46LnQ7E8QC4XpLuTuPD3S+IGVpUS/CQSb+fgOTC/AdoSXEwXqpTij0jTzSW+OsYZ8Jsqa4pHMtiZlT3ECn31/+JnSDTzSWJsgkI9ub/aSYQKH6JiDRfZnaURic+9g06zHEvLepxmbQA/tvzgFPW30s6JjeVNqDfl0uxjd6qrNKKQ+D47TgXSV+pQHUl7zPauRVrrg60tUh69O7bkoc0t2qQWC8Fg+UYHzAO31gQa9qjW3u3NAcWJEgBeXJbXdOdbycu9kcvWsjjK8l1a5IrcPrmVtsrIuqUJPnf4OnP3DDOlXRO/LeYkWTFX7zgPmetdfjJk07H1XQaCGpW7X54KrLkJEEQb8F/XNKsJYoKb2wbC04amNs4TP3MXQE/uLZfve1LncE7WeZCCl2uHeE2sz3h/zsRfoV69tHC9R3GU2rirYhSylC4Nnh9ZOyhi/JpU6TyHI8toTUWS6a0XtlVJB05913zWaIO9z1S4nGSaCW5H/+tE+bfRUAqLvXmLc8c7rGBwys1ns21AwB9oGM1eAI7GEdSABE+hc7lQDTBNg9a+OKxVX6DeUkZWK+t2BSmmJwJHrZ09e84KZmIhMiE369QLxC5K459hQ5/rf4RXvwXuOsog0Rrk05p/LBAYrT959VH+EkJmlVo83oIkeSqKz6C4Nbdf4MSGBLmKq+CqPJ29u24dFkt52D4iHwfyn4hagP6aXcKrTzIRJNCdB/nHV9kJNbjq/2aFKJUicTKiICRrc1wN62eJz3CH9aAbT9OgKhlYanfW9+yBVZOxwAJeazVDkR+pKLk7oqB1BoVi3r+96dSXZ0dM1eu7+JicX98qP+IXti6QhcRvNuOMHy0z73tO+B1xzukXO8IezUo38LA/XHdh1PPTjgvyShT89DJOQffvtfOnM3mSfHf+lr+LmSE7H9ensgrxEu1E3f9KHn6tuNCN8O6kDzQBH1XTXlN8wGnqSYN2O7CHjNUoUROqrkaW4mbhcSYgbMULyn9qGV3UAAqcR7BTzclPLFxSnhfPzA1ThK+QAJASQ6LgbJwDHz7w8AhzZ9Lo9chyAC7i1Ep7l4xNvSnrR1Lnzs0dVmNZ/LR3Jo4zAgmgWgr4ygbzcnbLuYrQlmfccVuNXwti4QzRdug/Styehu1NnTKzY9xdwoMyD5qgwa7mILv2ZqZ+TIZebWEGUE+77IctaoDOs5w//06vsmLTOToKeI8dLqPio7FHfIJZieyCoBxuFPgpQa5R9j0ApuVDVJ0Vf/lcsD3EncF5pgpfkDz7AUHPmkxV/8OrsL+yrLyHPAiHJqoFiiBGcdACwTdHrMKQuhpYUcIi3AvQd+GP85jg1wOUolbs2SGQpG35aq5xkgTilANoe2Hwr7WMe44QU5oN63038YJceHIiLl4JkdhpnJOtnWdkmPWBuzWfQUE9XJDtOOX1a9DF7KR+4NwystTtJIH3dbOIgG4F3V6V67uEzZgy18B552VurBn6/qrQt+mqxxd3gQYR+1gOOSxPa35r5Ti02wJRv5fsy2kJehagb08X2PU9Ne0PZI9jWfK8u2UmQIO8w3XZWfO6oIxBOarIb6EEU3A9CvDlxVgplUGBPlzwih21BHvY3FVvg7EAFpRFN/MLyYF+N2Y1ENXm8BzwrRuDtJbXlGxpynfnOrgrs79uDQ5+76NDJiCyV750flVkNh1wi6CWgVJzm4NV2gJg937iNjThCSjFzHNNxJzHfqLEUaq/RhqQM51XftPvbFHccLLdYfsAWiT8xpUFm8cSCj4hkipFGGsLArqAhDq/lyMNHZuGWefOCH1APF2yo+jPgrVJFoGMPpFT+jgxepeBYyQUkEaUO6fgvirEPw18bJDPyhU3ynGVusiawzAff/MnNlrIX9auVQO2+dF3sIcF5o1xe4i6myWLwpoeUpuXb1r+bxoQZDwGSHEX/Tol7+8WmyBld3GrH+lWia3V4QgpiArkAr8eazY4ahwnIdQxjIBgc5593tvpj89nRusgNr13q0Huq0zyewNiz/ApomurTT37MnTlO73HTTLHn8RSlFSfDcSUmlmAnM/Kvjw56k90xsyHOgPf3YSM51+tEdaXM8wILh1jbCx6deDdA6NLTjBf9iLLZ7oJYti8d7P4YBKcptdxPwNCHIOQTXdJEehSnN0HEsNH1egQhh5eiWHmNxPSrJ91y/pWhOqgLCUNJYDuKE5CeD6tIrcpX5YNeUPEdM/AYP840dZr7eYTrAvE3YcI0p3D51WbQdpGjHL6oJNBkoFlPxS0RUlG/l2war3NOcZBn39zTS/hbNaMgj1Q+V9kX6sAeQWQk0KclOO6gHjTGUQQig9k14m0cTe4Hir45GUYERn2TfudxtkytOacjG6qczt9917F4RwEtpCUKeDiFFM93QdHeHiHSEBh9eqGtCbJoMUHG7t0oEGCGq9xJa6rChPEuKr4LGaiW8imM9kYOHmB95PrDS6tOK4J9xDS76vNo8+HMM5Emi936uxi/ialaiqJPI2f+TB8YrzZxZ3OMCzyDyrnT/WNICEgt0dQqeKriBhD9kjKgicRxzxsQ1VjlBjt3Ep2nGDg+HznoRYGZUMmOmdrMLoNX7mD+vTBQjRi6iS2dWC+fkaCm9blDx3LrgWtgJeYqeUxRChbH/fo2e6fRkPPgeU+cQf/hhJPMtySW7578gwV03l4Qo3xM4bueuNx8X+SK6hYwcB2GphT0T9mvkPcYhWRZdzK6x19FDFvz8xXwA1Hn0TBwDdyG6XD+zcSz9VKPQjAE2lCYZrcH9L/SCpV/8mKiVIXGRrm5KY3JFwhOAMOohH442Xhwm+7nzK04j60MDE6KpLm/jYzcPTW3+13wZ22mSsndAdu9J4ovL+id/l9RZAXWVPxdtmwNCcesFID/43ik4h/x4QjeOV4DXcDFIMTaFM+iFeAAAAAAAA"
              /></a>
          </b-col>
        </b-row>
      </b-container>

      <b-container>
        <b-row>

          <b-col>
            <h3>
              <li>ZilPay</li>
            </h3>
            <a href="https://zilpay.xyz/">
              <img
                alt="Zilpay"
                src="data:image/webp;base64,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"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>CoinRequest</li>
            </h3>
            <a href="https://coinrequest.io/">
              <img
                alt="Coinrequest"
                src="data:image/webp;base64,UklGRjgKAABXRUJQVlA4ICwKAAAQOQCdASrIAMMAPpFCnEqlo6Khp3IaKLASCWVu3V7XN0V0lIXX//7uSgfzz0V+in9+9Xb1dbvHHOb5L+1/3TREvajlAMs/3Xs47CdqL1WntHwWgD838+eaJ+kMKhrnj01CulKU1FTpVwLA38yg6rh1HVZHzOVhM52LzixBcEmOwb3fMQ1upsTK4a0VZfII1XnYifJ+nd3VOOHhD6vgBQVnaetEYM5WOKyuSGqWgQRnEmOwbufcg+l81d5vXTrCj8wqn4Fo/1h/ymr0jFfq2qd+caqVVA68uqKDnHic0P3H4aurHwMttP8FDHbG5Y+oz9kkAoZy7GzvzwaKbDq9/YXNP7M5i2lrSbk6rlj5zI05vyFVdAw+weYCrxzb1+Q6a0UcSq4jaFq3RBRe+dzSTuU72LSXeipByYbdOeHA3deiTmpJgMvnJtQipH5613m6CNuinDi4EKyMLkowspw0fI2Hcmx2RlfxSTll2k40qau2nXo+incjqYQIIo0YaDmIa3PpjAtdUFKRuaHY2XGbUPMClvSnf3tkrK6mv8Z6qsit1sS9hSCulsuL0g6CqCc/QEa/Ytm4K7rKJ8KV9+7v5rAfuv5Wb3KsBK3dx3u+WE8W6AAA/vpSn2+YcFNxL/+4Gv+kztmMBnsvyjbDzH6qqJCy1paQunRW6weAhvACgeKa2P/ojdKrZ+wkAlYfc/3T9VyOYtTZS12Kwo1b66w07DrQsbB7Fxeaf/zlhH4c2Q/g1yLK6CNm0F4KVtzQX7WV+YyoVyT6VdfnIrsC50RSG7gcETnE9GoJVlvTosfosPH44ydXjlDJZh1YhmUG60GSmIXhhrnpgYUGTDSlNyYsLR47GtxZYjr/eT/aIcI8aP2U9F0vokJb9RJw5r9CslwYZvdU/3+OU+Sm997AlifhBsVE095fxp33TaBbp8afB/IWoPK4mwuQDrLE2tpjAQyKKK0dm/bslxUxrb/Y1zAaCG2QWdAwF5rwBjCaIFq4OIxniXgE93JXOMVHGmJGGSwsFKHaHcApbTCX93U9HFQigG+i9JdEVVcNzwjh501oM7gMLAB6F1+1uFVu9wi5bGne6JhJPLh9msRz0JnXCqwpbwDXAZgkmmVe07rnwRRptcwxPYCK52E+xiByxQuzMGZkiO+7iOT6HuyMpXd00H50WaHxqLca6LgikcC/1b2EUmVV+3qonJLBA3/mUA1RttSJZ4yX1ZxMTWL74bGPWGCWSH9G+uMEdxaPgSTDncN+1/kcL2zGA20Wxv+tD6xD3tpwfV5GR+c17dneiIi2YYv2vbdlpJyN5N700p54J2jgoftdj6pQIEcBy+SVShpWopVEcZfhsL8iapdpe9sLFEXa0CS+SvEAx+XVNxAvwzqhi9PJaAXiyW7IJXrp6YqItY/pWTZLlOk3h6ksx5UWCXlx7HkgiifDqX8XA7FaK2dPAc/sfbix7ASZ/UqATcyTG5dDIsnOIwo8q0MvI5xULjNDX9IJJn7fSLp/aqqbjqxLjGt8bVRDnpVHpQsgtoq2hbV/0mOlcQEnv5GI7/iQGGcbaKm10/V7Nm8nkCJJzCE2YxTv6n5R0KvQspFBMIPJK+bdTSKrVnpPskfavGceRBPj8Fo/YTj6Kob9UWC91Roq3OopIOa11dhOHssT0h4OwOKjRgW35XpUmFbvLgxlW7huflQkzsV5bvTPMhPQwzMKk1j2d3pit1TPsbLP71viekCvIQpgwsHDfppQi4ITuHizRzpTDRS1m1rjM4J0tiNpm1nvAOle+uMQ+QwVbQf0cMBaW4KEr7no03wsNep5K/XGqpVIC1InbuqfB03OhfVfB6/3XLMZJ0HK1F3C3zsdmbrcmsPJourMh4TWlmjnYqMaLy5R1KxCZonxFUcvRIgynSq6A+ufQzl3S3pPyYUaD6qJ9xvkqTvd2YOQRy0GG2+MSus0f4vxLxiuYcdxS6o2qYJWaIr9ya2urzuRnGDJRduN+Al8DAWBrz4V2dWiY8mQuLZNtqUbtx4j8uFelDYv+8+b1StM/sEFD3rORjY+bbu4J6LqZBMr0/ilUwHm+m9p5LSKNDbRULCrxoGX8fd/sCYIxFP7YemL6CikiR0QgLz2aI1NcdwOTQPPDLIw8PKm2PfEAY4JMukXY+VNSWL3W/oplh6i3a7YCySf8T2CVYxkTddmx3i48kmmB7KhJdlEIsTk+rTC10suvOZs2XdgGL20cL74NA1ZfDPM3ltjdKiz/4zV9jZGxcz+R5Yzt7yJGHR/ad3BH6+W3m836/HIL6tMXZ6y2NlfxYrV/lQNXXu71otnS8q7EbEfmL9J4eUkb3SOGhgA6/iZaaAytma4syRcSTJ6VP+MIMhu0GEEtErIhcGdP+bj3vY3dPkvleGtQnH7/cerTymmvF+4E1BKemumzPx1TToEKGglABcYsAHJfNSHdfAp3MZYNpB2mLqPGnJ/UOUgIhvBv0lYJ2hWVnoqrjDaVcr/zwNFDNFVzlU14pd9paDcOKQzoEr4NS7yi2eDTRsv1eC10gawPAcsFQ/eNJXxRs6CINJjqjcQ1xg9Y/BQYkmfJb+4RJOvGF9juRz7Ueunjxg49kmwCUPsPTfL+SU8uVd1OFyxYY4eprB+5ODW5bmU6/h5e58+8Wf9Nrp3FL1O54ehX3QzwpgRqYvnrpr8X4KB24IzGePrPSTGCFHtcg9BvrreXjmGoemiRTth2cHWc5d1CRoq8Uk0HPxn959q+hzDrk4mHj35AfOEH+VgEWcFeuSZN8L0bM1gQgavAcYsFlrIn2nLc2/bD0rAyRcdoEsRxPXfNLaiDIiIVC3MLJhRHFMfvhr7SiYuA05eDvdF/Wl1TZgnwnRMsFBfeDOPCgl5AbT3yZl5Avb2fRHagOX+NEckIi3j+RPPt6h4D+Qyl7clCsCo0VJu1oozX1gMp0WP0WHp0WsDyW2nvp6IseqfSsExbtYqdAmqMF4AJmTkfm5DlljFkTc5LeAH0QGSqGiYnaJ3jBt0dTjCRptLVAxOhDGd1hmd7gIyIqTXKeIHbEJUYEQg8t6YKadZa2p1KU1liNBxovqie9xjZ33Vq7DwmpYsps75YXCkdwjP/kI7K1p9jwjPTdhJrwBjCiQAsZgzNqPdAY08uI8JdWq0rnrAzs8+KLcswFEwEf6o9LrzLdh1W5WRGoQjuCTWSOtfO9D3xLTGbKAnILOy1pSoWf9Tjq6o8mMm37Z/PZTUaJSxapm78RUhL4n9rWjVSf8t/J9oy4AX43TlBkvTIjFKdKMGwDDnB+B+axwB+SwsFKITI1vw/sIFkKOH7ujtN0pW6rcrU+BO9uecJPggUxIPlVFgBAj67r281nDU33Nz3c/DvrmjWDKRvG/AjgJ5IvUKJfYaZoCZOvIc78Feq12XIDLLajWJrSJCvwAQMp1EBWYV1Hxg1g30cWHNHvxrB5FF8lfrPwN0x5bLRQlAzQCxMaARj2H7UDwAAAA="
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>ViewBlock</li>
            </h3>
            <a href="https://viewblock.io/">
              <img
                alt="Veiwblock"
                src="data:image/webp;base64,UklGRjIMAABXRUJQVlA4WAoAAAAQAAAAxwAAxwAAQUxQSBQFAAABkEZbt2k3O6ztoLZt21ZS27bdhrVt27Zt24yt/aPeZ+9dd0TEBMCfv5lrVa9es+iPgCsi4okfAZePjv0wHP2flQk/CJbWEz86YWuttcR5qrYfvXDb6St3vD4KunP1zM4lrp1q5E+uqGQVeiw59yIIv3Hw68sr+lVztFRPospjD7xHgt6np9S1V0zadhteIWHvnX0yq8Su3W4/JB98qFd6ZViXW/IaDfXZXC+mHhJ0PItG3x7goIMUI56g8e8mZpEv+fDnyGLA3KyyxRvyDNn09XSQy6LFXWT1eb+YQhU8iOxerCpRXJcgZDhyoZ04ZS8h00+dZbEdH458L0woSNajyPrtkmI4vUXmA3vLYDEuCvlfEluA+BtRxBPp2Et3HoV8VIS5/I9RzA81WCv/DgUNdmasvA+KGtqVrfLeKGxUT6bKe6O8nVgq64UChzgxlOslihxSjZ2Ud1DoD4WYiXUCxb7vyMsyFPxoTE4GoejzGKkSKht2YsPxKQrvV4CLbSj+1Tg89EYFTmchl68GImswYHUIVXg3kXndUYnTjUv7TguhJU1bgWo8ZmVW2Qg9YDujLI+gIh8mMMkZVTnCINsLunhjZ04TVOZYY2wvaOONvSlOqM5hhlgc08eD+GaUjtAHtjVjBSr0lIUJaX00ElnahL6o0nkGWJ/VyYvE9ApH6gSb0HNBpa4jF+2KVt7bUSscqRV0pjYY1bqE2gG9PIxFy95bL+FFadVExfajNUEzW2gd1szD2JSSvNJMcF5KxSM0g86UWqNqXShN1M0OSrt1c8OWjs0N3bx2pOPwSjdh+ejkCtENVqdTBpXbgY6TdobT6a6dGXSGa2cVnana2UNnvnb2frP4+6595RUv7QRcvXrty0+m/lSiN6j84Myfeao9n0w/Gonfai8ky6didBzQ/8t7ntHOvd79+n/xgO4JP/UNZ2tnF5B10c52OkO0s4BOO+140qmunQF0ikQpx4lOJl/llKKT4KFuArLRgTO6eZyI0DLdnAbCA3WzmFIt3fSmlMlPNZUoRbujGa/UlGCtZs4D6Z6amUqrcLhinGjFuK8X/7S0YJFejgDxZnoZSc3+g1YiClODjVq5ZEOupVbGAXm79zqJLEgPVujklKUB1XTSDQyMcV0j7+xMgH4amQ9G2r/VR1ghM2CaPnaCoVkCtBFZ1RRYpo0DYGzeYF1EVTEHFujiABic0VcTkZVMAjdNrAejEz/Wg39Os6CtHsaB6fu0cCeecbl8dRBVE8wfroOlwKDNcQ3cS8YB5PCWL6Ia8NhZPjfgcql0h63ZiHdJthfpgc9c7yULqwqc1gkTrC/w2keu6cDtRKk2WLIDy2Q6EAf4tVov0YWkwHHcvfJcsAee4+6R5oI9cB1rlSxn7YFvqyWS7IkPrLvLsTIWMN89VAh34L/6Gwn824OEWU/zd78UyBh7Jncb7UDMFm84C+oHkmbcxdf5wiCrRQ8vngJdYoG4mdZzdLgIiFzvOjdPO1mB0HEGvOTEzz05CO7g4cVFwNysIHxqj3cc+M3JCgpMOey+aS88s4AS47U4GmHQuW7JQJEWBSbeNePFgrI2oM04VWc/ovZiSb1EoNO4Zcad9Kbid9mjRiJQbfr6rkeeR3ynV6dnNMliBRpOnt953LpT972+zvfxuW1uLYrYg64tEqXOVbZ+lw4HPrrfsWvDCrnTJbEGxY/56DD8ALp8dPR/iDw+OvMj0PHE8eMnZvwI/LIHVlA4IPgGAACQJgCdASrIAMgAPpFInkslpCKhpPO5oLASCWNu4W0Q65p/5buMw9+q5ezm2NO+jf99CP559AD9Dusf5gPNr/Gb3pf+H1AP/X1O+8hfun6FHX89IP1C/rHbxXl/5rhB2rP8FvXcCv7vXMTV/HvqADiZmZmZmZmZmZhyeWZmZmZcG7UfD+jitmqew16yoUnlYAZOGZl1So+PiLM09ZJOO5/VDL6HlQA72F/80VtbeDz+DlQr4JQHJXDf/tWwOoA7tcYSfS0eO1JUGCL4JcfE7f+Dbu1gaZ6qc1WRHCAWAJL8u/Ulj+BnWMyimodKBD8lyntmzG18p0LMv9xCgpbKgoJGD33QNefz0Cyyqs5cI9lPj0oXZkPibJr+RKuiBMzMsBO1dIALzanzOGG4qxWru7u7vBEwDu7u7u7u7u7sgAD+/ngAABUd+unqCyOIOAFWt7+BnCgLWC2v9o3xhvIwUeAIJKZMpBxVEuTIyAeZaTq4VpzIzPTt8YazROwnkx+pSjnwJoEn243nMijwuMz2dJty1z5m6t3mNeM1L0Xdvk/gCYl37IS1T+KgJ0BwDGw065sKlao9tNgKHYv03R42zQSaNdq2nX68Zcdfvoi8peavnMghBi2PQkyaTmhM0l0TEImHndQmmY2TnO4IbvAD87c87jXCpYe5XwARk+5jIc9NNrRUO/HqCALaN6oi9jLj+vUl7ivcF10oRhVJmxOZUAZS5U8/jOM2J9DU7upeT5ZS5exDixAXkvI0u0QyXCSR/LkN2pXtzIzqgV4RBHE7QPsHjnnX/UGaVvhw43CUMrxIeN6DrLnW3ofwG1Q0E1Kn55oTwBotFIeEcvYja4Edkq7w+shRPD5Y8FndMls45qO9+w4CkMwBFpfBoa6e3iA9sh1+W7sk1kItakeRzM/NjrSad1Ijc06zrL2mnETCxNCREK6YY0zxJhv8NRzJsL6/rjd7K5FMcA/L9Hixkp4GCjSfb686mT5RG6KgFzGvtYd5+NOWJUN3w1dEqH6h3buKnrOlkxN5wmGlRWQpemVUsyxlhs/c214iRToQic9SGmsVnJSeUOyFesPBgKCvI9HbwEh8tkyel4daIM8kczwHQtXOAOOKxP6dzhdQCdCrhzOuwrPpStCpnOx56c/AmA2qiKlNLqvrLPyFZv7IkeqHvdHP9VpiYvrXtdLF0jhdLkOb4W9l886EFdCdpOXqmJF4bFC6VSIbI8W3Kbeb40baJwD1VUjVgai9ca8QE9OD8edWFMPMbTzG1UNDj/4prLMYnCotGHG94d7G3TUVpJ2fWF8vaL2+vvLP3OCGJStLJ3cz3NcMc3Q0P+QpY5eIsSZc3WKOo3dN3srDylXRKNvqnjfQBgXOClM0rV8SqGpEaJ29sBcBKFpkXaoyFGwTCSRwp3hi2A0wWml6BVtS38RVKV40Ha+0a/jg3o8qGTU9NF7Ca7XAAaa1/73uSZRJkG6j0ay4EEke5uriKZWG4i05pWuUb1MuFG7rzyrEz08xhNmTtQTViqIeh0Fp8kFsLAe697l18nZzTsumEDE4M7IrqC6LQ/BTROdkp+f1N4rHqYGVpAEcqLwnL6GZEMRwu375J9QOqlX40IHcbXpk1dmw7pwEtlbzCmL/XXqnq3uod/yy4Z37ua/IagvX1wLGqsibXXsK2QwoqZqH+p3M0xVPNZnZmefZi574ZTbWVm/8xW5Wq4LQsEQtN/8hiRthSlHwmkAzczD6A11LOw1JCGI+nCBKil9oAe1sbRR9T5Rps8hj2X3sOl00x190mda1QBrj31V+N5WqhevYTcu1v0tvqhg58kQ72BR+xk/h/Yx3wTAdjSX0ASQvh+j+yfLqbNzfHp3z7QRCt686YL64tQXrI0y/50EuRZWQV8y6Hb1rucnDQKORhnyJBjHf2wJghEIJw4Q6eQ2f/xPf1UYMxCAiospEZNkyizHT30zpPjGXhR01ooh/MAiNwE6zoDguymzeJQiqkyroXaIj0pPW9SuWWqTXK17qWThI4fCXFHgUkZV07VBIdeccBMJQtfCyEQRHpBZD0APHexOKF5X8F0J0KtaGqRXLcP4av9oSN8B3DJCp36vwyZyH/i+nYKm5In4u57X73gE5xXtLwaOkpGGlH/MjgI4HUD1/TathtnYTm+nPjzfAXki2rCFoPR7SMsckLe6z1Uls6GBHut/gtIWhCFdfWgihtXHnnVlvec/tyPDiZ5sj5mHsZ5wAR4Ywp+kOwHxOi8uIFSj8eb5gXNuTpg0nN9008z2alz0t6gJ2uQWnpL81M5tg46DwsHnRDNavFNVKQZq/lt2zfTEbtOe7uwBV9ZuGt/BjydUg3D5qwrDj3e8mGaGwM3V5myCYGkhtP/cAAAAAAAAAAA=="
              /></a>
          </b-col>
        </b-row>
      </b-container>
      <b-container>
        <b-row>
          <b-col>

            <h3>
              <li>TrustWallet</li>
            </h3>
            <a href="https://trustwallet.com/">
              <img
                alt="Trustwallet"
                src="data:image/png;base64,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"
              /></a>
          </b-col>
          <b-col>

            <h3>
              <li>imToken</li>
            </h3>
            <a href="https://token.im/">
              <img
                alt="Imtoken"
                src="https://ens.domains/static/imToken.2f7546bf.png"
              /></a>
          </b-col>
          <b-col>
            <h3>
              <li>MetaMask</li>
            </h3>
            <a href="https://ens.domains/static/metamaskmobile.e382144e.png">
              <img
                alt="Metamask"
                src="https://ens.domains/static/metamask.e382144e.png"
              /></a>
          </b-col>
        </b-row>
      </b-container>

    </section>

    <br>
    <section>
      <hr>
      <h1 class="display-4">Get your blockchain domain!</h1>
      <ul>
        <li>
          <a href="https://unstoppabledomains.com/r/e8542f2138624e1">
            <b-button variant="danger">Visit UD</b-button>
          </a>
        </li>
        <a href="https://www.facebook.com/pages/category/Information-Technology-Company/Unstoppable-Domains-437586016802082/">
          <li>
            <font-awesome-icon
              :icon="faFacebook"
              size="lg"
            />
          </li>
        </a>
        <a href="https://medium.com/unstoppabledomain">
          <li>
            <font-awesome-icon
              :icon="faMedium"
              size="lg"
            />
          </li>
        </a>
        <a href="https://twitter.com/unstoppableweb">
          <li>
            <font-awesome-icon
              :icon="faTwitter"
              size="lg"
            />
          </li>
        </a>
        <a href="https://www.youtube.com/channel/UCg3gV2yVjRytsgpc1ZPiqjg">
          <li>
            <font-awesome-icon
              :icon="faYoutube"
              size="lg"
            />
          </li>
        </a>

      </ul>

    </section>

    <br />

    <cc />
  </div>

</template>

<script>
import Navbar from "../components/Navbar";
import cc from "../components/cc";
import pricec from "../components/Pricec";
import udcara from "../components/udcara";

import { faYoutube } from "@fortawesome/free-brands-svg-icons";
import { faMedium } from "@fortawesome/free-brands-svg-icons";
import { faTwitter } from "@fortawesome/free-brands-svg-icons";
import { faFacebook } from "@fortawesome/free-brands-svg-icons";
export default {
  name: "ud",
  components: {
    Navbar,
    cc,
    pricec,
    udcara




  },
  data () {
    return {
      faFacebook, faYoutube, faMedium, faTwitter,

      items: [

        { message: "Premium domains" },
        { message: "Grant program" },

        { message: "Domain management" },
        { message: "Self Custody" },
        { message: "No renewal fees" },
        { message: "Smart escrow" },

        { message: "Readble human addresses" },
        { message: "Build uncensorable website" },
        { message: "Accept over 50+ different crypto payment via domian" },
        { message: ".ZIL variant (Zilliqa blockchain)" },
        { message: ".CRYPTO variant (Ethereum blockchain)" },
      ],

    };
  },
  head: {
    title: 'UD Overview',
    meta: [
      {
        hid: "2",
        name: "description",
        content: ".crypto, .zil, domain"
      }
    ]
  }
};


</script>

<style>
html,
body {
  width: 100%;
  height: 100%;
  margin: 0px;
  padding: 0px;
}
.ud {
  background-color: #5c03ff;
}
.display-4 {
  text-align: center;
  text-shadow: 2px 2px #344a5f;
  -webkit-transform-style: preserve-3d;
  transform-style: preserve-3d;
}

.display-4:hover {
  -webkit-transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg)
    rotateX(-180deg) rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg)
    rotateZ(0deg);
  transform: rotateX(-169deg) rotateY(174deg) rotateZ(0deg) rotateX(-180deg)
    rotateY(0deg) rotateZ(0deg) rotateX(0deg) rotateY(180deg) rotateZ(0deg);
}

h2 {
  text-align: center;
}
@media only screen and (min-width: 320px), (max-width: 360px) {
  .display-3 {
    font-size: 150%;
  }
  .frame {
    overflow: hidden;
    width: 130%;
    display: flex;
  }
  .container {
    width: 100%;
  }
}
.frame {
  justify-content: center;
  display: flex;
}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {
}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {
}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {
}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {
}

h1 {
  text-align: center;
}

li {
  justify-content: center;
  display: flex;
}
img {
  height: 101px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
