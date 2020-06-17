# 인공지능 사관학교 프리코스 과제 목차

## 2주차 과제 (2020.06.17)


{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "name": "2주차과제.ipynb",
      "provenance": [],
      "collapsed_sections": [],
      "toc_visible": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "tMEA4LyXqBOz",
        "colab_type": "text"
      },
      "source": [
        "# 2주차 과제\n",
        "- 파이썬 문제\n",
        "- 인공지능 수학 문제\n",
        "\n",
        "\n",
        "*주의사항\n",
        "\n",
        "-- 문제에서 제시된 변수에 저장된 값을 __직접__ 변경하는 것은 오답으로 처리됩니다. (__예외도 있으니 문제설명을 자세히 읽어주세요__)\n",
        "\n",
        "-- 제시된 변수 이외의 변수를 추가해서 문제를 풀어도 됩니다 (__문제 설명에 명시된 변수 변경만 불가합니다.__)"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "z1qTsPAIkmfA",
        "colab_type": "text"
      },
      "source": [
        "## 파이썬 문제"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "Lqd5sxxas0rW",
        "colab_type": "text"
      },
      "source": [
        "### 01번 문제 (Data Type)\n",
        "\n",
        "__다음 변수 a, 변수 b, 변수 c의 자료형을 출력하세요.__"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "R8MW9Rqhu61b",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "962852cd-2a1b-4669-e0db-93afe3340e8b"
      },
      "source": [
        "# 주어진 변수(a, b, c) 직접 수정불가\n",
        "a = 'str'\n",
        "b = 123\n",
        "c = True\n",
        "\n",
        "\n",
        "print(type(a),type(b),type(c))"
      ],
      "execution_count": 4,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "<class 'str'> <class 'int'> <class 'bool'>\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "1gR8X465xuCj",
        "colab_type": "text"
      },
      "source": [
        "### 02번 문제 (for문)\n",
        "\n",
        "__다음 변수 num_list에 있는 요소를 모두 더한 값을 for문을 활용하여 변수 answer에 저장하고  그 값을 출력하세요.__"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "wI7l2ltaRUKy",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "3ccfc1c8-d069-4a40-db20-7957cfbce580"
      },
      "source": [
        "# 주어진 변수(num_list) 직접 수정 불가\n",
        "# for문을 사용 하지 않은 경우 오답처리\n",
        "num_list = [1,2,3,4,5,6,7,8,9]\n",
        "answer = 0\n",
        "for i in range(len(num_list)):\n",
        "  answer += num_list[i]\n",
        "\n",
        "print(answer)"
      ],
      "execution_count": 16,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "45\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "PtKl46h3S4wL",
        "colab_type": "text"
      },
      "source": [
        "### 03번 문제 (slice string)\n",
        "\n",
        "__다음 변수 date를 슬라이스해서 year(년), month(월), day(일)를 각각 출력하세요.__ (출력 : 2020 05 11)\n",
        "\n",
        "(tip: None을 지우고 date를 슬라이싱해서 각각의 데이터를 저장하세요!)"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "270XbDvYqvJu",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "2b874a72-51d2-4c4f-e4d4-e11474646452"
      },
      "source": [
        "# 주어진 변수(date)만 직접 수정불가, 다른 year, month, day 변수는 직접 수정가능\n",
        "# 슬라이스를 사용 안 할 경우 오답처리\n",
        "date = '20200511'\n",
        "\n",
        "year = date[0:4]\n",
        "month = date[4:6]\n",
        "day = date[6:8]\n",
        "\n",
        "print(year, month, day)"
      ],
      "execution_count": 58,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "2020 05 11\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "sOjirt93r2Ob",
        "colab_type": "text"
      },
      "source": [
        "### 04번 문제(for)\n",
        "\n",
        "__다음 변수 summary에 1 부터 100까지 모두 더한 값을 저장하여 출력하세요.__\n"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "MiGjtBg3r2f_",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "7887107d-c523-4b3d-dcd0-37e4b1019f65"
      },
      "source": [
        "# 주어진 변수(summary) 직접 수정불가\n",
        "summary = 0\n",
        "\n",
        "for i in range(1,101,1):\n",
        "  summary += i\n",
        "\n",
        "print(summary)"
      ],
      "execution_count": 19,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "5050\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "g-nnpUwya5Lp",
        "colab_type": "text"
      },
      "source": [
        "### 05번 문제(string reverse)\n",
        "\n",
        "__다음 변수 hangul의 문자열을 거꾸로 출력하세요. (출력:‘사바마라다나가’)__\n"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "hHCquVTHbSNN",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "70c10e66-b259-482a-e717-e87b080e0708"
      },
      "source": [
        "# 주어진 변수(hangul) 직접 수정불가\n",
        "hangul = '가나다라마바사'\n",
        "\n",
        "\n",
        "\n",
        "print(hangul[::-1])\n",
        "# 출력"
      ],
      "execution_count": 43,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "사바마라다나가\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "uUQ7rQWeclz5",
        "colab_type": "text"
      },
      "source": [
        "### 06번 문제(str -> list -> int 변환)\n",
        "\n",
        "__다음 변수 num에는 공백으로 구분된 4개의 점수가 들어 있습니다. 평균을 구해서 출력하세요.__"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "kcUrhpt5c22W",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 226
        },
        "outputId": "865b82da-e193-491a-cf5f-f70ac8b61cb6"
      },
      "source": [
        "# 주어진 변수(num) 직접 수정불가\n",
        "num = \"70 50 90 70\"\n",
        "\n",
        "#출력"
      ],
      "execution_count": 107,
      "outputs": [
        {
          "output_type": "error",
          "ename": "TypeError",
          "evalue": "ignored",
          "traceback": [
            "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
            "\u001b[0;31mTypeError\u001b[0m                                 Traceback (most recent call last)",
            "\u001b[0;32m<ipython-input-107-048ba501a196>\u001b[0m in \u001b[0;36m<module>\u001b[0;34m()\u001b[0m\n\u001b[1;32m      3\u001b[0m \u001b[0;34m\u001b[0m\u001b[0m\n\u001b[1;32m      4\u001b[0m \u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0;32m----> 5\u001b[0;31m \u001b[0mprint\u001b[0m \u001b[0;34m(\u001b[0m\u001b[0mnum\u001b[0m\u001b[0;34m.\u001b[0m\u001b[0mindex\u001b[0m\u001b[0;34m(\u001b[0m\u001b[0;36m1\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m)\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n\u001b[0m\u001b[1;32m      6\u001b[0m \u001b[0;31m#출력\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0;34m\u001b[0m\u001b[0m\n",
            "\u001b[0;31mTypeError\u001b[0m: must be str, not int"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "167vtalddRGH",
        "colab_type": "text"
      },
      "source": [
        "### 07번 문제(if문)\n",
        "\n",
        "__다음 변수 n에 입력한 값이 짝수 일 경우 ‘짝수’를, 짝수가 아닐 경우 ‘짝수가 아닙니다’를 판별하여 출력하세요.__ (출력: __짝수__ or __짝수가 아닙니다__)\n"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "8gwIuAVWdl9Z",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 53
        },
        "outputId": "b7bbaf70-7638-46ef-c104-e85f0dafc178"
      },
      "source": [
        "# 주어진 변수(n) 직접 수정불가\n",
        "n = int(input('숫자를 입력해주세요'))\n",
        "\n",
        "if(n%2==0):\n",
        "  print(\"짝수\")\n",
        "else:\n",
        "  print(\"짝수가 아닙니다\")   \n",
        "#출력"
      ],
      "execution_count": 25,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "숫자를 입력해주세요37\n",
            "짝수가 아닙니다\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "QLySHJw9eB01",
        "colab_type": "text"
      },
      "source": [
        "### 08번 문제(산술 연산 및 list index)\n",
        "\n",
        "__직사각형의 대각선의 길이를 구하는 공식은 밑변의 제곱 + 높이의 제곱 = 대각선의 제곱이다.__\n",
        "\n",
        "__다음 변수 list_08에는 하나의 직사각형의 밑변과 높이가 저장되어 있습니다.__\n",
        "\n",
        "__각각 밑변이 3이고 높이가 4일 때, 직사각형의 대각선의 제곱의 길이를 출력하세요.__"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "9bEv0Wn3e_Da",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 35
        },
        "outputId": "991d2281-cb39-4396-c153-ecd929674e0d"
      },
      "source": [
        "# 주어진 변수(list_08) 직접 수정불가\n",
        "list_08 = [3, 4]\n",
        "\n",
        "a = list_08[0] * list_08[0]\n",
        "b = list_08[1] * list_08[1]\n",
        "\n",
        "c = a+b\n",
        "\n",
        "print(c)\n",
        "# 출력"
      ],
      "execution_count": 74,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "25\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "efgr8XT3j0QE",
        "colab_type": "text"
      },
      "source": [
        "### 09번 문제(소수 판별 프로그램)\n",
        "__입력받은 숫자가 소수인지 아닌지 출력하는 프로그램을 작성 해 주세요.__ (출력 : __소수__ or __소수가 아닙니다__)"
      ]
    },
    {
      "cell_type": "code",
      "metadata": {
        "id": "j7MNZZGGuXu0",
        "colab_type": "code",
        "colab": {
          "base_uri": "https://localhost:8080/",
          "height": 53
        },
        "outputId": "3528cc05-3c04-4dad-b42b-64ea7dc53d0d"
      },
      "source": [
        "# 주어진 변수(num_10) 직접 수정불가\n",
        "# 함수(prime_number) 직접 수정가능\n",
        "num_10 = int(input('숫자를 입력해주세요'))\n",
        "\n",
        "def prime_number(n):\n",
        "  a = 0\n",
        "  for i in range(1,n+1,1):\n",
        "    if(n%i==0):\n",
        "      a += 1\n",
        "\n",
        "  if(a == 2):\n",
        "    print(\"소수\")\n",
        "  else:\n",
        "    print(\"소수가 아닙니다\") \n",
        "\n",
        "\n",
        "prime_number(num_10)"
      ],
      "execution_count": 84,
      "outputs": [
        {
          "output_type": "stream",
          "text": [
            "숫자를 입력해주세요6\n",
            "소수가 아닙니다\n"
          ],
          "name": "stdout"
        }
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "tN2dx7b0gHM3",
        "colab_type": "text"
      },
      "source": [
        "## 인공지능 수학 문제"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "QshpWJfxfO6A",
        "colab_type": "text"
      },
      "source": [
        "### 1번 문제 (Hypothesis)\n",
        "\n",
        "다음 공식은 Hypothesis를 구하는 공식입니다. 다음과 같이 값이 주어졌을때 h(x)의 값을 구하시오.\n",
        "\n",
        "*   W = 3\n",
        "*   x = 10\n",
        "*   b = 1\n"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "upv_hWgL8yks",
        "colab_type": "text"
      },
      "source": [
        "# $$h(x) = Wx + b$$"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "ZFMYPx42mt2E",
        "colab_type": "text"
      },
      "source": [
        "#### 정답 : 31"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "6sIvtew0eHSy",
        "colab_type": "text"
      },
      "source": [
        "## 2번 문제 (Cost function)\n",
        "\n",
        "다음 공식은 Cost를 구하는 공식입니다. 다음과 같이 값이 주어졌을때 cost의 값을 구하세요.\n",
        "\n",
        "* W = 2\n",
        "* x = [2, 4, 8]\n",
        "* y = [5, 12, 21]\n",
        "\n",
        "(tip: x1=2, y1=5 / x2=4, y2=12 / x3=8, y3=21)"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "tjWpl4O1oXy1",
        "colab_type": "text"
      },
      "source": [
        "# $$cost(W) =  \\frac{1}{n}\\sum_{i=1}^n (Wx^{(i)}-y^{(i)})^2$$"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "ITWV0EuznYgF",
        "colab_type": "text"
      },
      "source": [
        "#### 정답 : "
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "sQMi2ASxeJtt",
        "colab_type": "text"
      },
      "source": [
        "## 3번 문제 (Logistic regression sigmoid function)\n",
        "\n",
        "다음 공식은 로지스틱 시그모이드 함수입니다. x가 __양의 무한대로__ 갈때 f(x)가 수렴하는 값을 구하세요.\n",
        "\n",
        "![대체 텍스트](https://prwatech.in/blog/wp-content/uploads/2020/02/logi3.png)"
      ]
    },
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "e_e_z3PCkDgM",
        "colab_type": "text"
      },
      "source": [
        "**굵은 텍스트**#### 정답 : 1"
      ]
    }
  ]
}
